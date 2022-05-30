---
layout: post
title: Why all animation studios have the same org chart
date: 2021-07-05 13:32:20 +0300
description: Why do all studios (animation studios in this case), have the same org chart. 
img: orgchart.png
fig-caption: # Add figcaption (optional)
tags: [Management, Studio]
---

I posted this question on Twitter the other day:

![](/assets/img/twitter-studios-orgchart.png)

But it is something that has been bugging me for many years now. Why do all studios (animation studios in this case), have the same org chart. Of course, there are always some minor differences, but I'm talking about the big picture here. Departments. Head of departments. Project managers. Different seniority levels like "junior" and "senior" and so on. If you have worked in one it is like you have worked in all of them. Where did this structure come from and why are we all using it? It would make sense if this particular structure was perfected for years and it naturally evolved over the years AND if all studios are producing the same kind of projects. But that's not the case. I haven't seen this structure evolving much if not at all. And what's even more bizarre is that even new studios that are started today are organized similarly, regardless of the actual work they do. Big studios, small studios, studios working on series or commercials or feature film productions, studios in Africa, studios in Europe, studios on all continents. It all feels like a copy of itself.

Just to be clear, I'm not saying that there is something wrong with this structure. If it works, then let's use it. But it kind of feels to me that we are not even asking or discussing the questions above. It is the same as the QUERTY keyboard layout. They were invented almost 200 years ago to solve a mechanical problem, yet we are still using them, even though they might be more awkward and painful than a Dvorak layout for example. I'm not advocating that we should all suddenly switch to Dvorak. What I'm trying to do here is to just point out that this is something we collectively invented and that maybe other even better alternatives might exist. And to not talk blindly here, I will give an example with one very particular part of this structure - one in which I have been involved for years and give you some alternatives to at least think about. Here is how characters are created in animated movies (not including hair, cloth, shading, etc. for simplification):

![](/assets/img/orgchart-01.png)

 
The yellow boxes are different departments. A character is first established in the Story, then the Art department creates a design for it. The design is taken by the Modeling department and a 3D model is created. Then Rigging takes that model and creates a rig for it, which then Animation can use to animate shots with. You can see how nice and sequential everything is. The downside is it rarely works smoothly like that even though in theory, that's what this org chart is supposed to do. Here is what happens on a daily basis in reality: 

A rig is broken in one of the Animation shots. A mail thread or Jira ticket is created for the issue. Rigging investigates it and finds out it is a problem with the model. Sends the issue back to Modeling. Modeling fixes it and sends it to Rigging, Rigging updates the rig with the new model and publishes a new version of the rig which then Animation can use to fix their issue. First down the chain, then up the chain. When other departments are involved like character sim, hair, and shading, then the chain is even longer. 
Rigging starts working on a new character and finds out the proportions of the arms are not going to work for Animation's purposes. The issue gets discussed in a number of meetings with the Modeling and Art department which they agree to fix by asking the Art department to create an updated design for it. The design is updated, the model is updated, the rig is now using a new model and Animation is happy.
Art creates an amazing design for one of the characters. It gets modeled. Then rigging takes the model and spends weeks trying to come up with some solution of a crazy armor piece on the shoulder that breaks every time Animation does something with the rig. 

I have seen some studios trying to resolve these issues by doing some minor tweaks to this structure. For example, Pixar is known for merging the Modeling and Rigging departments into one (at least when characters are concerned). So instead of two yellow boxes, you have one yellow box in their place. Other studios are adding some additional roles between the yellow boxes that need to take care of some of these issues. A role that takes the model before rigging and makes sure it meets the animation and rigging requirements. Some other studios are better at collaboration between departments and spend more time iterating over the deliverables before they are delivered to the next yellow box. But this often doesn't fix the actual problem, which is that the structure above is the culprit and causes many undesirable and less visible side-effects: 

Problem ownership. Because all the yellow boxes are a bit isolated and self-contained, it is hard for someone to fully own the problems when they arise. To be honest, in some studios the departments actually feel like different small studios operating inside the big studio. You will often hear sentences start with the word "they" when something is broken. The issue is often kicked from one mail thread to another mail thread and from one yellow box to another yellow box until an "owner" of the problem is found. 
Trying to synchronize work that way from a Project Manager's perspective feels a lot like playing Tetris with Gantt charts. Work needs to be reshuffled in order to make space for fixes, which in turn slows down other work and other departments, and so on. 
So the time to deliver goes up and throughput goes down. 
Project Managers become micromanagers. "I know you need to work on character A, but can you squeeze in fixes for character B as it is needed by tomorrow?" 
This in turn creates frustrated and disengaged artists and morale go down. Remember - autonomy, mastery, and purpose. 
When autonomy is taken away, artists will leave the company. Or worse - they will stay but feel disengaged from the actual work.  
When artists feel disengaged from work, innovation suffers, and mediocrity reigns. 

It is a self-reinforcing loop. And like all self-reinforcing loops, changing one variable in the system can lead to either instability or stability. Imagine instead a different structure. One where instead of having different departments working on the same character asset, we minimize the number of dependencies to the minimum. So for each character, we have a team that handles it.

![](/assets/img/orgchart-02.png)

This team consists of a Designer, Modeler, Rigger, Animator, and if needed - a Character Sim artist, and so on. The team is responsible for this character from start to finish. When a fix is needed, the team handles it. Give full autonomy to the team to manage themselves and find the best solution in any given moment without much politics and Tetris playing. Scheduling between the team members is done internally by the team, no need for a coordinator to micromanage them. Needless to say, the team can work on several assets at the same time as well, but it is up to them to decide how to best do that. 

This is also a simple test that you can try on any of the characters your studio produces and see how it works for you. If done properly, I'm positive the effects would be noticable.


