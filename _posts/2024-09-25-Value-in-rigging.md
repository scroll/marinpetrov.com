---
layout: post
title: "What is the value in rigging"
date: 2024-09-25 22:47:00 +0300
description: "How to think about value when prioritizing rigging tasks"
img: scrat.jpg  # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CG, Animation, Rigging]
growth: 1
---

When teams prioritize development tasks and projects for rigging they often forget about what makes an item "valuable". Should the team value more an estimated 2 months initiative to optimize the rig speed by 6% over a change in the spine component requested by animation? How about fixing a bug that should probably take a day or two, but is breaking the whole studio pipeline. Should it stop every other development currently in progress? In an ideal world we will do everything, but with limited time and resources, it is important to prioritize properly. But we can't prioritize without understanding "value". 

In this blog post I will try to tackle down a common misconception I see in rigging teams about what actually constitutes "value". I am intentionally going to leave out the concept of "urgency", because I find that it is an easier concept to grasp. Although [both should go hand in hand when you prioritize development](https://cutlefish.substack.com/p/tbm-245-the-magic-prioritization), for now I will just focus on the "value" concept as it's a bit more tricky. 

First let's start with some first principles about rigging. 
1. **Nobody needs rigging**. This is a hard truth to swallow if you are a rigger. Or a liberating one if you choose it to be! Let me tell you a personal story. More than 20 years ago, I decided I wanted to be a character animator. But back in the day there were no rigs you could just download and start animating with. So in order for me to start animating, I first needed to create a rig for a character I also modeled. Think about this for a second. What I actually wanted back then was to animate, but what I ended up doing was creating some bones and skin in order to animate. The same is true with any movie or game production - if there was a way for an animator to animate without a rig, they would do it. Not even the audience sees the rig on the final screen. The only purpose of rigging is to help animators do their job!

2. **Rigging's value is measured by animator productivity**
The ultimate measure of a rig's value isn't technical elegance or code efficiency—it's how effectively it enables animators to work. A "perfect" rig that animators find unintuitive or cumbersome actually has low value, while a technically simpler rig that animators can use efficiently has high value. Value metrics should include: animation speed, quality of resulting animation, and animator satisfaction.

3. **Value exists in context**
The same rigging feature might be critical for one production but unnecessary for another. A film with a lot of character performances needs sophisticated facial rigging, while a racing game might prioritize vehicle deformation systems. Value assessment must consider the specific production needs.

## How to increase value

So taking those principles, you can see that value can be created in many different ways. 
For example, we can choose to do something which will **increase Animation's productivity**. Things that fit in this category:
- Improve a rig component to allow easier and faster animation
- Increase rig performance
- Create a new deformer that makes it easier to achieve a certain pose

We can also derive value from initiatives that **increase production speed**:
- Rigging framework to make authoring rigs easier and faster
- Pre-made archetypes
- Tools to facilitate deformation work
- Universal meshes

We can take actions to **reduce bugs**, basically costs that we are currently incurring by producing rigs which are not "per the standards". Initiatives in this category include: 
- QC frameworks to catch bugs early
- Standardize rig creation

And finally value can be increased by **avoiding bugs**, basically reducing costs we are not currently incurring but may do so in the future: 
- Maintain readable codebase
- Unit Testing
- Metrics dashboards to check rig builds
- Reduce code dependencies and complexity

I also think that if you want to deliver the most value, you need to choose initiatives that check more than one of those boxes.



## Common Value Traps
Rigging teams often fall into these value assessment traps:

- **Technical impressiveness bias** - Prioritizing complex technical challenges over simpler solutions that would deliver more value to animators.

- **The "cool factor" distortion** - Pursuing exciting new features while neglecting maintenance that would deliver more overall value.

- **Invisible value blindness** - Undervaluing work that prevents problems (because avoided problems are invisible) while overvaluing work that solves visible problems.

- **Specialization silos** - Failing to recognize value across disciplines because riggers don't fully understand animation workflows.


