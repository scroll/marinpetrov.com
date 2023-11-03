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

Many animation and VFX studios surprisingly don't measure their production in terms of performance or implement any metrics at all. Frequently, the only "metrics" that get measured are deadlines for various tasks. Imagine you're driving a car with a goal to reach a certain destination, but the only information you have is the current time. You lack knowledge about your speed, performance, the remaining gas in your tank, or even a GPS to guide you to your goal. The chances of reaching your destination when driving blindly like this are slim. In this post, I want to introduce a few metrics that can provide a robust understanding of how your rigging pipeline is performing, where you are currently and where you want to go next. I'm focusing on the rigging pipeline here since that's my area of expertise. So, this post is primarily for those who work in rigging departments or those who oversee entire productions. There may be other metrics you'd want to measure if you're a modeling supervisor or you're working in another department, but that's a topic for another post.


## The importance of metrics

The answer here seems fairly clear. To borrow from the car analogy, if you're driving and wish to reach a certain destination, you'll need to measure your speed and direction at the very least. Without that, you'd end up somewhere random, possibly somewhere you don't want to be. The same holds true for any rigging pipeline - tracking the right metrics can help you evaluate the effectiveness of your rigging pipeline. These metrics enable you to monitor your progress — are your goals being met? They also help to identify any bottlenecks and inefficiencies in your production. Utilizing these metrics allows you to make the necessary improvements and maximize your return on investment.

## What should be measured?  

When it comes to rigging pipelines, there are four metrics that are crucial. These are indicative of the speed and stability of your rigging pipeline.

- **Rig Failure Rate** 
- **Time to Resolve Issues**
- **Rig Delivery Velocity** 
- **Feedback Response Time**


## Rig Failure Rate 

This metric calculates the percentage of rig publishes that cause an issue in production, requiring an immediate fix. In essence, it measures how many of your published rigs are broken.  A low rig failure rate is desirable because the more time a team spends addressing issues in published rigs, the less time it has to deliver new rigs or improve rigs in production. It is measured as a percentage with the following formula: 

*(published rig failures / total publishes) x 100*

This metric provides insights into:
- the effectiveness of your QA methods and practices
- the stability of your rigging pipeline codebase

I've found that effective rigging teams typically score between 0% and 12% on this metric.

## Time to resolve issues

Rig failures are inevitable, but how much time does it take for you to fix them? This metric measures the average time for all your rig issue fixes. It's calculated by measuring the time it takes from when a rig was found to be broken to when it was republished and fixed.

This metric indicates how effective your team is at addressing issues in production.


## Rig Delivery Velocity

This metric measures how quickly a team can deliver a rig to production. The faster a rig can be completed, the better. Of course, different rigs require distinct timelines. A basic biped character will take much less time to deliver than a complex, lead non-biped character. The best way to approach this is to measure it for all rigs in a certain production or production period. Record the time a rig's creation is started (the first rigging work file is created) to when it is published. If your rigging pipeline operates in stages, measure this for all the stages, giving you a granular perspective on the metric.

This metric reflects how effective your team is at the most crucial task - producing rigs! 


## Feedback Response Time 
This metric calculates the time it takes from the receipt of feedback (from a supervising animator, for example) to when that feedback is implemented, and an updated version of the rig is published. You want to minimize this metric as much as possible. Measure it by recording the time a rig update based on feedback is started and when it is published to production.

This metric gives you insights into:
- how effective your team is at incorporating animation feedback into the rigs
- the adaptability of your rigging pipeline to implement such feedback


## What to do once you start monitoring those metrics

After implementing these metrics, you can review them at the start of each weekly meeting. You and your team will want to continuously work together to improve these crucial metrics. Any initiative or project you undertake should aim to enhance these metrics, not weaken them. This approach will enhance the decision-making process, helping you prioritize and focus your efforts. For example, if your Rig Delivery Velocity is improving, but there are many broken rigs in production, concentrate on refining your QA methods. If too much time is spent implementing feedback from the Animation Supervisor, focus on the capacity of your pipeline and team to deliver changes faster.


---
*If you are someone on a rigging leadership position, I would love to chat with you about all of this. Are you currently measuring any of these metrics? What are the current metrics of your team and how are they improving over time? Did you do something specific that affected those metrics positively? How about negatively? Reach out to marin@hey.com and drop me a mail to chat.* 