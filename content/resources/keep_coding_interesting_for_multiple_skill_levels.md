+++
title = "Keep coding interesting for multiple skill levels"
slug = "Multiple skill levels"
tags = ['scratch', 'python', 'robots', 'codeclub', 'maker']
description = "During a meetup, some questions came up about catering for a variety of skill levels in Code Clubs. I thought it might be useful to share some of the ideas that came up as well as some tips from our experiences at our Code Club, where we deal with a variety of experience levels and ages across a large group."
+++


![screenshot](/images/warp_zone.png)

## Guided learning verses multiple stream choices
In our own Code Club, we've taken a few different approaches:

- picking out individual interesting projects from the Code Club curriculum each week;
 - following the curriculum in order;
 - providing a variety of activities that provide students with skills ranging from various forms of visual coding to 3d design for 3d printing; and
 - providing short-term workshops that apply coding skills, in areas such as robotics and web applications.

These are some of our experiences with each of those approaches.

There was a tendency for some students to gravitate toward the less code-orientated activities. At first we thought that this was a good thing. I mean, they were engaged and learning some skills. Of course this is a good outcome - but what happens when the same student wants to build a robot, or has an idea for a new feature, after only doing 3d Printing? For this reason, it's been helpful to keep kids doing the Code Club curriculum long enough to get a good grounding in coding before tackling other areas. To make this work, especially with larger groups, the ability to help kids quickly with any questions that come up and potentially slow down projects, is important. As a volunteer or teacher, taking the 20 minutes to complete the activity beforehand makes a huge difference to how quickly you can assist or walk through the troubleshooting process. In order to do this, timely notifications to volunteers or teachers of upcoming projects will give them more flexibility to schedule a time to go through the projects themselves, prior to a session. A free collaboration platform that works on mobile devices as well as computers, allows sharing of tricks and tips, while providing a common notification channel that is easily accessible at convenient and flexible times; for our Code Club we started using a free [Slack](https://slack.com/is) with only 2 organisers, and ended up extending a subset of this to volunteers. Other alternatives, such as hipchat, are available. The important thing to consider when choosing a platform to collaborate on is whether it is easily accessible by your team and within budget. Although a share group chat on SMS could work, the advantages of these other solutions, is that they allow integration with other systems e.g. file sharing, calendars etc. and it is easy to paste documents or photos. It's important to remember privacy rules that apply to information - so use the same rules as for any online service i.e. don't post personally-identifiable information from other systems.

In our first six months of running a Code Club, we focussed mainly on visual programming with [Scratch](/python/code_club_and_programming), picking out interesting projects from the [Code Club World Curriculum](http://projects.codeclubworld.org/en-GB/), answering quesions as they came up. It wasn't long until we had a few students make their own games, that they showed to the group, and this resulted in a few more games being written. This was great to see, and the kids that already had a grasp of coding principles did really well. However, subsequent questions that arose pointed to some gaps in skills due to us too eagerly skipping through some of the Code Club projects. One challenge is that we progress at different rates and students start out with varying experience levels. Other factors included available time, access to computers and Internet at home, and the amount of assistance that friends or family are able to give. Since we generally have a set group of students who attend each session, there is the opportunity to get to know where everyone is at individually and, to a limited extent, give them projects that fit with learning requirements. This isn't always the case, and so often a catch-all approach of having everyone go through the curriculum in order, can be a way of minimising gaps in knowledge and skills, while fielding questions that also give insight into whether a student a new challenge. A key ingredient to this recipe is having material to cater to those students who move faster, or already have skills and don't need to do some of the projects. Having said that, our aim is really to give kids an understanding of programming, not just to let them be programmers, but to allow them to know what can be achieved in order to give them more opportunities to harness technology. Whether they end up marketing or designing, having the appreciation and ability to communicate with coding e.g. quick prototyping or demonstrating, can be a valuable base and inspiration to launch other endeavours. At a minimum, it's great to see students with at least enough knowledge to conceive innovative projects then collaborate to make these work.

## Branching out
Once students have a reasonable grasp of basic programming concepts it's great to reinforce those skills by applying them to their own projects, but soon it will be time to branch out to making more useful software to create some practical solutions to problems.

Some of the useful concepts that can be learned from visual programming e.g. Scratch (Tickle to a smaller extent) etc. include:

 - iteration e.g. loops such as `repeat..until` or `forever`
 - variables e.g. keeping a score during the game, or waiting until a specified number of chances have run out before ending a game
 - list structures e.g. creating and manipulating lists of things such as names
 - branching i.e. making a decision to change program flow based on conditions using `if..then`
 - nesting i.e. putting branching or iteration structures within other structures
 - simple functions e.g. creating a new custom command in Scratch to handle jumping

A number of volunteers have expressed frustration with trying to wean kids off visual programming.

A few useful benefits of moving away from simple visual programming can be:

 - interaction with physical or other external environments including files, motors, lights, network services, sensors, and cameras
 - learning more elegant solutions for real problems, that can be used in more environments than just a browser
 - being able to model the solution to a problem more easily using inheritance object-orientated programming
 - using or adding to pre-written modules to allow seemingly complicated tasks to be performed with simple functions 
 - allow more advanced access to interesting hardware such as robots or add-on electronic components

In our Code Club we are lucky enough to have skill sets that cover a variety of areas. As soon as you locate these type of resources, it's a good idea to look at duplicating some of these skills across other volunteers/teachers involved with your team/club. By this, I'm referring to creating some sort of information repository with some training and collaboration where possible. Having said that, even if you don't extra skill sets, since the Code Club curriculum, or whatever you are using, is designed for kids, as an adult it's going to be easy enough to do yourself, and as I've mentioned there's lots to gain from doing this. Personally I've learned a ton from going through other peoples' projects and following along with tutorials on youtube, or just in books.

## Teaching multiple levels
So now we come to how to actually juggle multiple students running at different skill levels, at the same time within that one hour or so of coding. As I've mentioned to other teachers/volunteers, it really comes down to having something extra up your sleeve. I learned the hard way with a bunch of kids chomping at the bit while I'm trying to make things up on the fly, and help other kids, the more pre-written activities you have ready, the better. This could just be a matter of having an extra activity pdf ready on a file share or however you distribute these. Even if it's not a whole activity, it helps to have a list of stock standard challenges to use. So for Scratch, here's a few I suggest myself:

 - add a scoring system: use variables
 - work out how to add another level or more: broadcaste events 
 - extra features, such as new enemies/obstacles/tools
 - copy sprites and modify for 2 player: write scripts once, modify for second player and scale up the game to accomodate
 - convert variables like energy or score to graphic representations: use costumes on a sprite, and match the score or health to the costume number
 - add a menu: similar to the multi-level one
 - cheat mode, extra difficult mode, powerups

Something that Rik from Code Club UK reminded me of, is to always give the kids a hint, or at least make sure they have an idea of how to do the challenge. That way, you know their mind is already ticking over and they won't just be sitting there not knowing what to do.

## Encourage questions
At the other end of the spetrum, there are the students for whom things just don't make sense at one point or another. As most teachers will know, it's important to always _check for understanding_. The problem I've come across is that when I ask whether kids understand something they'll say "yeah", and then proceed to show that they don't quite "get it" yet. That used to be me, until someone explained to me that it was fine to say "I don't quite get it", because then they could teach me. It occured to me that often saying "no" feels like an admission of guilt i.e. not listening properly. Telling the students that there's no dumb questions, and sharing that I was actually the kid who "didn't get" things, helped with this a bit. Having spent a number of years selling in another life, I've learned that if I want to get a message across, it's my responsibility. Asking those open-ended questions can be great to both determine where a student is at with their learning, give you some ideas of activities to suggest, and better ways to explain things. 

Having a good knowlege of the activites you have up your sleeve is helpful if you identify larger gaps in knowledge than you can fix in a short conversation. That way, it's easy enough to just suggest, "ok, what about having a go at this activity here, because it shows you how to do all these things you're wanting to do?"

## When things don't work during a session
Whenever you're giving students additional activities, either because they've already mastered most skills covered, or they're catching up on something they've missed, there's a higher chance of things not working. There's lots of reasons why this could happen, one being that teachers/volunteers may be less familiar with the content not yet used with the majority of students. These days I find myself trying to be better prepared for things that fail. Luckily, I've found I have also improved at making things that fail less by:

 - having multiple sets of batteries for robots, and using a battery tester to ensure they are well-charged;
 - using an access point that I control, if I'm relying on devices that I can't easily test on the network provided;
 - having others review any custom activities before running them; 
 - keeping objectives clear and attainable at the start, so that students will be gain confidence by achieving things early on, before progressing to more involved tasks;
 - using computers I have access to outside of Code Club, e.g. Raspberry Pis or spending time testing on one of the laptop builds we're provided with; and
 - trying to have a simpler version of the activity that I can fall back to, in the case of partial failure of my environment.

In simple terms, have an extra activity that will in the worst-case scenario just work with basic functionality, but with scope for lots of additional challenges if things go better than expected. That way students who want more, will at least get an extra activity, and in the case that everything works *really* well, there's enough scope to accomodate that too.

## Multi-tasking with extra activities
Setting up lots of checkpoints where students get feedback in anything custom I write, really helps when delivering. This allows you to have students progressing with an activity, while allowing a method of checking that progress. e.g. "how are we going getting to point B?", or "Follow the directions and do X", which allows a bit of a chance to help others, or keep track of other activities that may be running. Timing is crucial, as having to fiddle too much with something can often leave students idle and getting distracted. Even giving a simplified description of what you're doing to fix something that's not working as expected, can keep students engaged. Although often it's just easier to have the more advanced students help others while you fix the issue in their extra activity. Either way, "would you be able to do this for me?" or explaining how you're fixing things, keeps the learning happening.

## Small diversions
When we've set up too many activities, we found some of our students were able to get engaged where they had previously stalled on their set projects. This seemed good at the time, except that the opportunity cost of that was that later it was very difficult to get them back on track due to missed concepts and distraction. Sometimes a small activity can work, but for us we have needed to communicate that it will only be a temporary deviation, and not a change in learning path. To this end, we have compared a number of different groups where we've more strictly kept to a logical path, and noticed that there is more focus with less distraction, resulting in greater options later due to a more complete base coding skill set.

In some cases, when students have created something in their spare time, we've done well by having them speak briefly at the beginning of a Code Club session. It's imporant to keep these focussed, as the aim is to motivate others, but not distract them or add confusion regarding the direction of learning. This is not to say that creativity isn't encouraged, but that opening things up prematurely has cost us later on, when we've had to backtrack to fill skill gaps.

## Charting progress
It's easy for extra work or good wins in learning or creativity to get lost in the activity and go unrewarded. We recently introduced simple logging of completed projects so that teachers and students can see their achievements, and it's easier to see where help or challenge is needed over each term. There's a definite advantage in making sure as many projects get to the completion stage, as it keeps the pace up, while enouraging some collaboration around troubleshooting and learning. I urge our kids to make the very most of their time and work our volunteers and teachers hard. It's great when they push us as I'll find myself writing more Code to answer questions or demonstrate concepts.

## Conclusion
To summarise this slightly longer post:

 - for groups that have regular attendees, sticking to a clear path of set activities helps prevent skill gaps later, and allows more interesting projects to be tackled
 - be ready to communicate (and demonstrate if possible) the benefits of progressing into more challenging coding e.g. from Scratch to Python, and set reasonable expectations that this will happen at a predicted point in time
 - do some extra preparation at some point outside of Code Club, to ensure you have extra content for both advanced students, and those who need activities to fill any missing skill gaps to catch up
 - as learning paths diverge, make sure you have clear checkpoints for objectives so that you can either jump between multiple student projects, or tag team another volunteer at various points
 - ensure that extra activities have a worst case path if certain things fail during the session, so that students will still gain
 - be clear that any small diversions will be temporary, so that there is transparency and clarity in learning paths
 - do the activities beforehand, to maximise the value you can offer to students during the sessions
 - encourage questions so no one gets left behind
 - harness show and tell in a focussed manner
 - and finally, chart progress and strive to complete projects.
