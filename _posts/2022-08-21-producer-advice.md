---
layout: post
title:  "Advice for Digipen Game Producers"
author: Russell Johnson
category: 
tags: digipen producers game-project
---

In my time at Digipen I was a producer on several Game projects. During GAM200/250 the producer on my team wanted to step down and the only person who was crazy enough to accept the role was me. With GAM300 I stepped up and formed a team that had several 300 and 400 students to do an Unreal Engine project.

Here contained in this post is my advice that is paved from my experiences and regrets. Heed my warnings (or not). 

## Cut a build for Milestones early
You should create a build for the milestone presentations typically 2-6 days beforehand. If you are using source control that supports branching, cut a branch off and somehow prevent others from messing with or deleting this branch. Have everyone on the team sit down and test all that you are planning on showing off and collect bugs to fix. The only thing that goes inside that branch is bugfixes related to the presentation. 

This prevents, I don’t know maybe a specific Audio Engineer, from trying to add a new feature 30 minutes before the Milestone 1 presentation and subsequently having said new feature crash during the middle of our presentation.

Stash a copy of the locked build in several online places (OneDrive, Google Drive, etc) as well as keeping a copy on USB thumb drives you carry to the presentation. Test the build on the same computer you are presenting on the morning of your presentation, just to check if anything stops working.

Locking release branches is a common thing in the software development industry. At my work we like to issue a code freeze 3 weeks before the planned release date. During this time QA and a portion of our developers will thoroughly test each feature (even old features from previous releases) to make sure nothing is broken and that there is no crashing that happens. Only critical bug fixes are added to this locked branch.

## Practice the Milestone presentations
Create your slide deck a week early and practice presenting with your team at least two times before the actual presentation. Also have each member go over their lines on their own a couple times as well. Each time you practice you will build confidence and reduce errors (like saying uh or stuttering) in the real presentation. 

I know this will be hard to schedule, especially if you have multiple disciplines on your team (artists, designers, etc) but this is the most significant thing you can do to drastically improve the presentation quality.

There will be team members who claim that they do not need to practice the presentation before hand, that they can ad lib better. People who are good at this are VERY rare, so no make them come and practice.

## Lock software versions
At the beginning of the semester sit down with the Tech Director on your team and write down the versions of all software and libraries you will use. For stuff that comes preinstalled on Digipen’s computers like Visual studio just use the version that Digipen uses. Mixing software versions is a bad idea, especially runtimes and editor output. Only update if there is a good reason too (like it fixes bugs or some other blocking problem). Then test everything afterwards to make sure nothing broke.

Keep a backup of all the software installers that you need on something like Google Drive, OneDrive, or another cloud storage service. Digipen started offering OneDrive to students via your Digipen Microsoft account so you can use that.

On my GAM300 project we had a problem with Wwise crashing on our Unreal Engine project. It turned out that the version of Wwise Unreal plugin we were using was drastically older than the version our BAMSD was required to use for our project. I have also experienced similar weirdness with mismatched Spine editor and runtime library versions. Do not mix software output and library runtime versions!

## Have some way of visualizing work progress
As a producer it is very helpful having a quick and easy way to visualize what current work is being done and who is doing said work. One easy way teams achieve this is by having a whiteboard at the team space. The whiteboard is divided into three columns, “Not Started”, “In Progress”, and “Finished”; rows are added to represent every project member. Sticky notes are placed on the board representing an individual task/feature. As the task is worked on, you physically move the sticky note between each column as needed.

There are online versions of this whiteboard method, commonly referred to as “Issue Tracking”. [Trello](https://trello.com/) boards are a great starting point as it is free and easy to get setup and running in a couple minutes. The industry uses a software called Jira but using Jira for a Digipen project is extremely overkill. Only use Jira if every single member on the team is ok with that and wants to put in the extra effort it is to use it (and trust me it is an extra effort). Use whatever method you think your team will stick with. From my experience teams that use Jira usually give up after a couple weeks and use Trello or a whiteboard instead.

Try to keep each task on the board as simple as possible. Break more complex features into smaller tasks. One measurement I like to use for Task sizing was “Could someone complete this in the single day lab time?” If not, break it into smaller pieces. 

Sometimes when planning things, you don’t know what sub tasks a given big feature takes (like “make a graphics engine”, or “create an event system”). If you encounter a situation like this (and you almost certainly will) track the planning work by creating “Research x” or “Look into x” tickets. Once the person who is assigned the ticket knows more, they should break the task into more tickets.

At the beginning of your weekly Friday lab spend the first ten minutes in a quick “standup meeting” with the entire team present having each member give the current state of what they are working on, and what they plan on working on next. These types of meetings in the industry are called “standup meetings” because they usually have each member stand up in a room or team space. Having everyone standing encourages everyone to be quick and not spend a long time on unnecessary stuff.

## Keep meetings relevant for involved members
Try to keep the meetings on topic, relevant and short. This is especially important during an all-team meeting that includes non-programmers like designers and artists. Some programmers like to get into implementation details and other unnecessary fluff, so it is your job to quickly reign them back on track. If they really need to talk about some technical detail with others, have them save it for the end of the meeting and allow uninterested and uninvolved members to leave. 

## Work on Milestone requirements first
Obtain the list of all that you need to work on for the next milestone. From this list create a pool of tickets (commonly referred to as the “backlog”) and when a team member needs work, they can take a ticket from the backlog. For each discipline work with them on their specific requirements because their project/game class might be different then yours.

Try to get some basic features up and running fast. What are common features of PC games? Think of stuff like main menus and a basic settings menu. Get basic versions of these features up fast so you are not scrambling at the last minute of the second semester programming them (has happened way too many times).

## Scope small
No, you are not going to be creating that open world GTA style game, nor are you going to be able to create 20 levels with incredible amounts of details. Scope small and then grow if you have time. Create a very basic and fun gameplay loop and then keep adding things IF and only if you have time to do so, and the previous features you added are completed.

From my experience designers love to get into incredible detail and plan lots of things that you will not be able to pull off. If you have Designers on the team, it is the Producers job to help reign them in and keep scope low.

It is much better to scope small and have complete and fun features then it is to scope large and then must scramble at the end of the semester to convert what you have into some semblance of a game. Everyone will be busy with finals and class projects at the end of the semester, no one has time to do said scrambling.

## Assume team volunteers are going to contribute nothing
This was always a weird thing that I saw teams do. Hopefully Digipen has cracked down on this practice but if they allow it (and you want to do it) then go in with the mentality that they are not a full member of the team. Assume that they will contribute absolutely nothing and be fine with that. 

From my observations volunteers tend to work at the beginning of the semester then drop out halfway through. Think about it, why are they not in the game project class in the first place? If it is because they failed classes last year, then that is a sign that they already can’t handle the Digipen work load. Volunteers in a more specialized situation (like an upper-class man or graduate doing specialty stuff) is rare and might work better, but keep this criticism in mind.

## Source Control backup
Be wary of Digipen’s source control, especially when using Digipen Perforce. Every year I was at Digipen (5 years) Perforce went down for 2-3 weeks causing the teams using it to lose work during critical times. Digipen’s policy (at least when I was there) was to not penalize teams for this, but it is demoralizing for the team when it happens. Keep a backup somewhere else if you can.

I have seen many teams during my time use GitHub or Gitlab (sometime self-hosted by one of the students on the team) and if you choose to do this then setup a system to automatically backup the current source tree to Digipen’s source control. GitHub and Gitlab have a feature to use auto sync every so often, but this requires a team member keep their login credentials inside those systems. Maybe Digipen will allow git ssh one day. You as the producer can also manually do this backup, just as long as it is being done on a regular basis.

## Keep a list of member's contact info
Somewhere safe stash a list of each member’s name, Digipen email and maybe their phone number. The Digipen emails are important because most project Milestone paperwork needs it, so it is useful to store this somewhere.

## Conclusion
Some of my favorite memories at Digipen are from the GAM project classes. They were a mix of shared suffering and valuable learning experiences. Take these nuggets of wisdom and use them to improve your GAM project’s experience.

