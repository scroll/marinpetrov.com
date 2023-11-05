---
layout: post
title: The only rigging metrics that you will ever need
date: 2023-11-01 18:32:20 +0300
description: The title of this post is slightly clickbaity. Yet, I do believe these are the only metrics that matter for your rigging pipeline. 
img: metrics-rigging.jpg
fig-caption: # Add figcaption (optional)
tags: [rigging, pipeline, animation, studios]
growth: 2
---

Many animation and VFX studios surprisingly don't measure their production in terms of performance or implement any metrics at all. Frequently, the only "metrics" that get measured are deadlines for various tasks. Imagine you're driving a car with a goal to reach a certain destination, but the only information you have is the current time. You lack knowledge about your speed, performance, the remaining gas in your tank, or even a GPS to guide you to your goal. The chances of reaching your destination when driving blindly like this are slim. In this post, I want to introduce a few metrics that can provide a robust understanding of how your rigging pipeline is performing, where you are currently and where you want to go next. I'm focusing on the rigging pipeline here since that's my area of expertise, but this concept can be applied to any department as long as it produces some kind of assets. So, this post is primarily for those who work in rigging departments or those who oversee entire productions. 


## The importance of metrics

The answer here seems fairly clear. To borrow from the car analogy, if you're driving and wish to reach a certain destination, you'll need to measure your speed and direction at the very least. Without that, you'd end up somewhere random, possibly somewhere you don't want to be. The same holds true for any rigging pipeline - tracking the right metrics can help you evaluate the effectiveness of your rigging pipeline. These metrics enable you to monitor your progress — are your goals being met? They also help to identify any bottlenecks and inefficiencies in your production. Utilizing these metrics allows you to make the necessary improvements and maximize your return on investment.

## What should be measured?  

When it comes to rigging pipelines, there are five metrics that are crucial. These are indicative of the speed and stability of your rigging pipeline.

- **Delivery velocity** 
- **Feedback response time**
- **Issues rate** 
- **Time to resolve issues**
- **Rig performance speed**


## Delivery Velocity

This metric measures how quickly a team can deliver a rig to production. The faster a rig can be completed, the better. Of course, different rigs require distinct timelines. A basic biped character will take much less time to deliver than a complex, lead non-biped character. The best way to approach this is to measure it for all rigs in a certain production or production period. Record the time a rig's creation is started (the first rigging work file is created) to when it is published. If your rigging pipeline operates in stages, measure this for all the stages, giving you a granular perspective on the metric.

This metric reflects how effective your team is at its most crucial task - shipping rigs!

You can also break and separate this metric further if you have different stages of a rig - Phase1, Phase2, Phase3 etc. You can then measure how much time it takes in general to deliver a rig in each of these stages.


## Feedback response time 
This metric calculates the time it takes from the receipt of feedback (from a supervising animator, for example) to when that feedback is implemented, and an updated version of the rig is published. You want to minimize this metric as much as possible. Measure it by recording the time a rig update based on feedback is started and when it is published to production.

This metric gives you insights into:
- how effective your team is at incorporating animation feedback into the rigs
- the adaptability of your rigging pipeline to implement such feedback


## Rig issues rate 

This metric shows the percentage of rig publishes that cause some kind of issue that requires a fix in order for the rig to be usable. In essence, it measures how many of your published rigs are broken. If the rig issues rate is lower, this means the team has more time to spend delivering new rigs or improve rigs in production. It is measured as a percentage, i.e: 

(rig publishes with issues/all rig publishes) * 100

This metric provides insights into:
- the effectiveness of your QA methods and practices
- the stability of your rigging pipeline codebase

## Time to resolve issues

Rig failures are inevitable, but how much time does it take for you to fix them? This metric measures the average time for all your rig issue fixes. It's calculated by measuring the time it takes from when a rig was found to be broken to when it was republished and fixed.

This metric indicates how effective your team is at addressing issues in production.

## Rig performance speed

Although this particular metric is not strictly measuring the rigging pipeline but rather the product of the pipeline - the actual rigs, some people convinced me to include it as well. This measures the relative performance of your rigs in terms of FPS (frames per second). The faster a rig performs in your DCC, the easier it is for animators to work on their shots and scenes. If a rig runs realtime, animators don't even need to make playblasts of their scenes, they can just play the scene and see it in realtime. This is a huge time savings for the whole production! You can use different tools and scripts to benchmark a rig once it has been published or just before publish time. Just remember to benchmark it after your optimization steps.  

The metric provides insight into: 
- the ability of your pipeline and codebase to create fast performing rigs
- the complexity of the rigs produced
- it is a good conversation starter with anim sups about what's needed - more features added to the rigs or better performance of the rigs. 

Rigging is always a balance between features and performance, but a good rigging pipeline is able to produce rigs with many features without sacrificing the performance. 

## What to do once you start monitoring those metrics

After implementing these metrics, you can review them at the start of each weekly meeting. You and your team will want to continuously work together to improve them. This approach will benefit your decision-making process, helping you prioritize and focus your efforts appropriately. Any initiative or project you undertake should aim to enhance these metrics, not weaken them. For example, if your delivery velocity is improving, but there are many broken rigs in production, concentrate on refining your QA methods. If too much time is spent implementing feedback from the Animation Supervisor, focus on the capacity of your pipeline and team to deliver such changes faster.


---
*If you are someone on a rigging leadership position, I would love to chat with you about all of this. Are you currently measuring any of these metrics? What are the current metrics of your team and how are they improving over time? Did you do something specific that affected those metrics positively? How about negatively? Reach out to marin@hey.com and drop me a mail so we can chat.* 