---
layout: post
title: Should you serialize your rigging data
date: 2020-05-31 13:32:20 +0300
description: Deciding if and when you should serialize your rigging data.
img: serialize.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Rigging, Pipeline]
---

This blog post is more about rigging pipeline patterns rather than how to actually do rig data serialization. For the latter, there are multiple articles on the subject and we are not going to discuss it here. So let’s talk about one such rigging pipeline pattern.

Before we dive in to explore it, let’s talk about a few requirements first. Regardless of what type of studio you work at - VFX, Feature Animation, or Games, it is almost certain that you probably have the requirement to rebuild your rigs. This is mostly a production requirement - if you want to stay competitive you don’t want to lose time and build your rigs by hand from scratch any time the production requirements for that rig change. Most probably you have some kind of framework or modular rigging system that does this for you. And let’s face it - rig requirements change constantly throughout the production so being able to push a button and rebuild a rig after the requirements changed is the most logical step. But being involved in multiple studios and pipelines during the years I have observed two patterns for doing that.

One we will call “rig data serialization” or RDS for short. This is a great pattern because it allows you to write to disk or a database any deformer data you might have in your rig asset - this includes but is not limited to skinning and weights data, deformer weights, blendshape data, pose reader configuration, etc.,  and then rebuild your animation rig without worrying about losing any of this data.  It is great because you are not confined to the limits of your DCC to store that data. You can back it up, share it with other team members, import it in other software packages, lay the groundwork for rig variants pipeline and it allows for something I haven’t seen employed much - allowing multiple rig artists to work on the same asset without stepping on each other’s toes. That said, this also comes with a cost. And unless you are Disney, Blizzard, or any other big studio that can afford to do this, you need to most probably take this into consideration when you design your rigging pipeline. Here are just some of the costs of going that route:

* Writing and supporting exporters/importers for any of this data. Nowadays it’s quite easy to just use JSON (plain text) or proto buffers(binary)  to store this in some way, but you have to be ready to support the tools especially when the DCC updates and your tools end up being broken.

* Backward compatibility. Making sure you can import this data in newer versions of your DCC is actually important. This sometimes can be extremely tricky unless you are using protobuffers which avoids this issue. 

* Syncing up the data of your rig with the rig itself. Every time you decouple some data, you also need to make sure you and someone else from your team can couple it back the same way it was before. This means making sure that you are actually importing the correct and newest data and not some older version of it from another asset. And that another rig artist can actually assemble a rig made by someone else.

* Making sure that your data is importable even after you have changed some of the rig requirements - for example, what happens if you exported your skinning weights data, but your joints change names, you delete some joints or you add some joints? Can you make sure your pipeline supports these very common cases?

* Sometimes, you might need a tool to view, compare (diff), and maybe manipulate the data you serialize externally. These are another set of tools to write, and support, just to be able to do that.

* Making sure that you write and support all the additional steps in your rigging framework that import/rebuild your deformation data. 

* Making sure even junior artists can export/import this data. Too often rigging frameworks require artists to write and script some logic in something like a post-build step in order to import back their deformer stack data. But not all rig artists can script or are comfortable doing so.


So if the RDS pattern works for big studios it should most certainly work for small studios too, right? Well, the truth is usually quite the opposite. Patterns that work for big studios most probably are quite harmful for small or medium-sized ones. When deciding what patterns make sense for my team, my approach usually has been to step back and look at the requirements again and what we are actually trying to achieve here. In the case of RDS, there might be many considerations about using it, and if you don’t have another choice, it’s a great pattern. But most studios actually do have a choice and if the only thing we are considering is being able to rebuild a rig when the requirements for the rig change, then there is a simpler approach.

One famous pattern that all programmers know and love is “minimize your dependencies”. In the case of a rig asset, the dependencies are all the data that makes the rig asset. The more you minimize them, the easier it is to support the rig and the pipeline itself. Especially if you don’t have the luxury to work in a 2000 people studio. There are usually two cases where we want to rebuild a rig:

* The animation control rig requirements change. This happens when there is a request from the animation department to add or remove (although I have never experienced the latter) functionality.

* The underlying model changes in some way. This can also include topology change.

Let’s examine both cases. 

In the first case, a change is requested to the control rig. Here, the only thing that actually needs to change is the control rig logic and behavior. We don’t need to update anything in the deformer stack. In this case you can treat the control rig and deformer stack separately and design your pipeline in such a way where it allows you to rebuild your rig without deleting your deformers. And I would argue that the best format for your deformer data is not some JSON or proto buffer sitting on your hard drive, but actually the DCC scene itself! What better format for your skinning data than the skinning deformer in your scene? It also comes with a full-fledged interface for debugging it - like skinning tools, API for accessing and manipulating the data, etc. If you need to make an exporter and viewer of your data that complex - you should be quite ready to support such a development overhead. There is no real need to export all the deformation data, delete the rig, rebuild the rig, re-import the deformation data when the only thing that needs changing doesn’t even affect the deformation stack in the first place. You will save yourself a lot of headaches if you can just rebuild the control rig and leave the deformation data in the scene itself. In fact, I can assure you that you can even do the same thing in the second use case as well, even when you need to accommodate a topology change in the geometry. An easy solution to this is if you import the updated model in your DCC, transfer all the deformers to the new geometry, and delete/rebuild the rig for the new geometry. Again, there is no real need to leave the scene or export your deformers externally.

The biggest benefit that comes with this approach is that individual artists can work on rigs without the need for someone else from the team to step up and fix a broken exporter, debug why some data that was exported just one version ago is no longer importable and so on. It makes the rigging pipeline much easier to support. It doesn’t require a whole team to support all the infrastructure that comes with rig data serialization.

So are you a small team or a big team? If you are a small team, then consider rebuilding your rigs without serializing your deformer data.
