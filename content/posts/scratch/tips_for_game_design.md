+++
title = "Tips for designing your first Scratch games"
date = "2016-05-12T15:24:00Z"
tags = ['scratch']
description = "Talking to our Code Club kids about their Scratch games, I noticed a few things repeatedly getting in the way when attempting to take an idea through to a working game"
+++


## The idea ##

Our Code Club is part of [Code Club Australia](http://www.codeclubau.org/) who provide some great resources that include some fun Scratch game tutorials/exercises. When kids are new to Code Club, the best place to start is by doing several of these step-by-step activities. Sooner or later the kids start to get some ideas, and start designing some of their own game ideas. It can be easy to stay within the safety zone of what we've done previously. Sometimes that happens, and while it is a nice and easy way to spin up a working project, soon we find ourselves thinking up more complex ideas and jumping straight in to build them.

Although there's a lot of tutorials and videos out there that show how to make something by following step-by-step, this post is more about the process of going from a idea to a working Scratch game. Ok, and on with the post..

## Getting more out of Scratch ##

Once we get to the point that our code gets complicated, it can be easy to lose track of what does what. At this point things can get overwhelming. It can seem like programming is a brain-melting pursuit, and it becomes frustrating, or just a whole lot of work to make our game do what we want. In this day of many distractions, it can easy to give up, move on to something else, go and watch cat videos. Although if you actually want to learn something, it might be better to go and watch a Scratch tutorial, like some of [Al Sweigart's](https://youtu.be/1eMGlhQXclI?list=PL0-84-yl1fUkall6a14nqzXpG79-RgI1F), which are well-paced and engaging. At Code Club it can also help to go and do some more exercises. Sooner or later, we realise that there are much easier ways of doing what we want, and this can make our code seem simpler and clearer. Maths is a great analogy when you think about how hard it was to do various calculations, until you worked out all these ways of visualising things in your brain, and it became much simpler. It is always great when I come across someone who looks a bit frustrated, only to see their face light up when you explain an easier way to do something.

A good resource can be other Scratchers, who post tips and answers to questions in forums, or make demo Scratch projects. You can look at their code, and compare it with other similar projects.

Here's an example of something that really helped me; at some point, I realised that once I created a working character, I could drag the scripts create enemies, and then use clones instead of lots of sprites, to populate my game. Before that realization, I'd find myself using way too many sprites, and thought that Scratch was so much more limited than it really is!

So some of the concepts that help us at this point are:

 - there's usually multiple ways to do something, and knowing the best way that is easy to understand and read, can allow us to make more interesting and easy to manage games without getting overwhelmed
 - if something doesn't make sense, we may need to see it explained in a different way

## Solving problems and debugging ##

Often, I see a common cycle of enthusiasm -> frustration -> problem solving -> satisfaction. When we start Code Club for the first time, a lot of us need to put our hands up when something just doesn't work. As we progress through the activities, we get to know some common mistakes that we make, and later we actually start to use tricks like showing variables or printing values to the screen to figure out why something doesn't work right. That last point is really important, because eventually our code, which may now be easier to read, more elegant, and simpler, can still be complex enough that some of these tricks are useful in determining what is going wrong, and where it is going wrong in our code.

I put together a document during last year's Code Club, with a few ideas for troubleshooting Scratch bugs. You can grab it [here](/pdfs/Finding and fixing problems with your scripts.pdf).

When I see kids getting to the point of comparing code from one game to another, or putting it isolating it in another project, or just tracing through their code, to successfully solve problems, it is obvious that they have grown from just typing in someone else's code, to actually understanding what is going on. There is a certain clarity that comes with this, and often we can visualise in our mind, some of the ways we could make something work. There is a certain level of maturity in our thinking when this happens which is both exciting and empowering.

## Recognizing patterns and models ##

So guess what? In order to keep getting better at coding, and increase how fast we can create, we need to continually put ourselves though this process of attempting to do something, running into a problem, and solving that problem. That's practice, and in the same way that other activities required more energy at the start, until we mastered them, coding gradually gets easier too!

And something that happens as we go through this cycle of solving problems and learning, is that we start to recognise patterns. Some example of patterns might be a common way to implement controls for a player, creating gravity, adding lots of game levels without needing so many sprites, wrapping the player to the other side of the screen when they reach the edge, and so on.

Once we see these patterns and implement them in our Scratch games, it's important to start keeping a library of these. Doing this will make it much faster to pgrogram lots more games in Scratch. A great way to collect short snippets of useful code is by using the Backpack feature. The Backpack can be found t the bottom of the screen when you log into Scratch online. There is a label at the bottom, with an small arrow to view it. By dragging yours or other Scratchers' code snippets into the backpack, you will have read-made code to drag into your project. How good is that? You can probably see the time this would save. In addition to storing code snippets, the Backpack can also hold sprites and images. A good use for this might be some key animation frames, or favorite custom backgrounds. Although you can upload these too, having them online means you're not tied to your home computer or one you may use at school or an office. For more involved features you might need to just hang onto the game you created previously, as reference for something that took you ages to work out. Sometimes this could also be a trademark feature that makes all your games instantly recognizable.

## Have a clear plan with milestones ##

Often I like to ask our Code Club kids to tell me about the games are creating. Many times when we get into this conversation, they can tell me a few details, but are unsure of the whole concept of the game. If we had an initial plan, we can usually go back to that plan, and compare how our coding is going. By having a plan, we can check whether our game works as designed, or if something needs to be changed. It also makes it easy to measure our progress. Sometimes game designs can be entires storyboards, with lots of different 'states' or possiblilities. However, in Scratch, it is best to keep our plan to a simple single sketch, wiht some words to outline what happens in our game. At the point where we draw up our first plan for our game design, we need to keep it really simple. This is so we can focus on getting the basic mechanics of our game working. It's easy to get a bit ambitious at first, only to find that our idea requires a lot more thought, so to start off, just keep it real simple. I noticed one of our Code Club kids has been creating what's called a changelog for each version of his game. A changelog is a record of the changes that have been added to each version of the game. That way, you can go back to the previous version instead of right back to the start. With each feature we add, we can set ourselves a milestone. A miltstone in this case, is a previously-defined point that we see as our next goal. An example could be the implementation of a new feature. So the point at which that feature is working, would be our milestone. It's a really good way to keep track of our projects and to help us work toward small goals as we add features and enhancements to our game.

So let's say your initial plan for your game design is a bat that flies around on its own, and your player has to dodge it. Pretty easy to do, right? But once you have this done, then you could add extra enhancements. Examples of these could be:

 - a time limited scoring system that resets at the end of each game, when a set amount of time has passed
 - a menu to allow different options to be set, with each option being a separate milestone as well
 - mulitiple levels, with the backdrop and number of bats increasing with each level
 - bonus objects that allow the player to swat at the bats

..and so on.

Here's an example of a plan I made. It's probably a bit more ambitious, and I ended up simplifying it, as some components ended up not really being required.

![Example plan for game](/images/zombie_game_plan.png)

And here's what it ended up looking like.

![Zombie game](/images/zombie_game.png)

As you progress with Scratch games, you'll start to find that you can make your initial plan a little more complicated, because you can use your previously-saved snippets to make building it easier. Just try and start with something simple as it is more satisfying to have a completed game than several projects you didn't finish because of lack of planning. I've made an infographic summary of the process [here](https://infograph.venngage.com/p/105387/basic-visual-game-process).



