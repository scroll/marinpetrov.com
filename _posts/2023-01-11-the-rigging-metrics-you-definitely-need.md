---
layout: post
title: The only rigging metrics that you will ever need
date: 2023-11-01 18:32:20 +0300
description: The title of this post is slightly clickbaity. Yet, I do believe these are the only metrics that matter for your rigging pipeline. 
img: metrics-rigging.jpg
fig-caption: # Add figcaption (optional)
tags: [rigging, pipeline, animation, studios]
growth: 1
---

Not many animation and VFX studios actually measure their production in terms of performance or implement any kind of metrics at all. The only "metrics" that get measured are usually deadlines for different tasks. Imagine you are driving a car, you need to reach a certain destination and the only thing that you know is the current time. You have no idea about speed, performance, how much gas you have in the tank or gps to reach your actual goal. I doubt you will ever reach your goal if you are driving blindly like that. In this post, I want to introduce you to a few metrics that will give you a very good understanding of how your rigging pipeline is performing, where you are currently and where you want to go next. I only want to talk about rigging pipeline here because that's what my expertise is - building rigging pipelines. So this post is mostly for people who work in riggin departments or for people who oversee the whole production. There are probably other metrics you want to implement if you are a modeling supervisor or you work in another department, but this will be another post altogether.


## Why measure anything at all

I think the answer here is pretty obvious.  In the car example above, if you are driving a car and you want to reach a certain destination, you will at least need to measure your speed and direction to where you are going. Without that, you will end up in a random place, somewhere you probably don't want to be. The same is true for any rigging pipeline - tracking the right rigging metrics will help you evaluate the effectiveness of your rigging pipeline. They will enable you to monitor your progress — are you achieving the goals that you’ve set out? These metrics also help identify any bottlenecks and ineffectiveness in your production. Utilizing these metrics will allow you to make the necessary improvements and get the maximum return on your investments.

## Ok, but measure what?  

When it comes to rigging pipelines, there are four metrics that you most definitely want to measure. They are tied to the speed and stability of your rigging pipeline. 

- **Rig Failure Rate** 
- **Time to resolve issues**
- **Rig Delivery Velocity** 
- **Feedback Response Time**


## Rig Failure Rate 

This metric is the percentage of rig publishes that are causing some issue in production that requires an immediate fix. In short - how many of your published rigs are actually broken. A low rig failure rate is desirable because the more time a team spends addressing issues in published rigs, the less time it has to deliver new rigs or improve rigs in production. It is measured as a percentage with the following formula: 

(published rig failures / total publishes) x 100

This metric will show you a few things:
 - how effective are your QA methods and practices
 - how stable is your rigging pipeline codebase
 
I have noticed that effective rigging teams sit somehwere between 0% and 12% on this metric. 

## Time to resolve issues

Rig failures are inevitable, but how much time it takes you to fix one? This metrics shows the mean time for all your rig issues fixes. It is calculated by measuring the time it took from the moment a rig was discovered broken to the time it was re-published and fixed. 

This metric will show how effective is your team at addressingn issues in production. 

## Rig Delivery Velocity

This metric measures how fast a team can deliver a rig to production. The faster a rig can be delivered from start to finish, the better. Obviously different rigs require very different time. A background biped character will take very short time to deliver, while a lead non-biped character might take much more. The way to measure this is to measure it for all rigs in a certain production or production period. Record the time a rig is started (the first rigging work file is created) to when the rig is published. If your rigging pipeline works in stages, measure this for all of your stages - this will give you a better granularity over that metric. 

This metric will show how effective is your team at actually the only thing that matters in your team - producing rigs!  


## Feedback Response Time 
This metric shows the time it takes from when a feedback is given (by a supervising animator for example) to when that feedback is implemented and a new updated version of the rig is published. You want to minimize this metric as much as possible. Measure it by recording the time a rig update based on feedback is started and when it is published to production. 

Measuring this will give you a pretty good understanding of:
- how effective is your team at implementing animation feedback into the rigs
- the ability of your rigging pipeline to actually implement such feedback


## What to do once you start monitoring those metrics

Once you implement these metrics you can review them at the start of every weekly meeting. You and your team would want to work together to improve them as much as possible in a **continuous improvement** fashion. Any initiative or project you tackle should better those metrics, not worsen them. This will allow you to have a **better decision making** over what is a priority and where you need to focus next. Your rig delivery velocity is improving, but there is a lot of broken rigs in production? Focus on your QA methods. It takes a lot of time to implement back feedback from the Anim Sup? Focus on the ability of your pipeline and team to deliver changes fast. 


---
*If you are someone on a rigging leadership position, I would love to chat with you about all of this. Are you currently measuring any of these metrics? What are the current metrics of your team and how are they improving over time? Did you do something specific that affected those metrics positively? How about negatively? Reach out to marin@hey.com and drop me a mail to chat.* 