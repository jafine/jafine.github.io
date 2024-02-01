+++
title = "Code Club and questions about programming"
date = "2016-06-21T17:37:00Z"
tags = ['python', 'programming']
description = "Code Club questions"
+++


During our Code Club sessions, a lot of questions come up. It reminds me of when I was at school and trying to figure out how all these pieces of information fitted together. A good analogy might be piano lessons: school kids can often find themselves learning piano and doing exams, without anyone ever stopping to ask them what they wanted to get out of it or how anything they learned would help them achieve anything useful. In this post, I'll try to explain the why of some fo what we cover in our Code Club.

## Scratch 

Scratch allows us to visually learn programming principles and structures, and can be used online or install to run stand-alone on a computer. It doesn't take much to get quick visual feedback from Scratch, and doesn't need too much specific knowledge to get started. However, when we get more ambitious with Scratch, things can still get complicated. At this point, it can be easy to assume that Scratch can't do what you want. But when we look through video game history, there's lots of examples where developers have managed to squeeze a whole lot out of computers and consoles that we previously seen as limited. Although Scratch isn't any where near as complicated as the Commodore 64 or the PSX One, there's a big difference in how the more experienced programmers do things. Usually their code is much easier to read and understand, and there's often less of it. A lot of this comes down to good design and thinking ahead. In some ways, this is the next level of Scratch programming.

Although the 1.4 version of Scratch is outdated, since it was written in Python, it can be extended. Version 2.0 of Scratch is available online, and the stand-alone version runs on the Adobe Air runtime environment. So there are still some uses for version 1.4 by extending it with Python, to interact with external devices. It is also the only version that will currently run on the small, low-cost Raspberry Pi computer, out of the box. By leveraging Python plugins or scripts with Scratch, we can use our Scratch skills to interact with more than just the visual and audio of the Scratch environment.

## Python

Python is essentially a text-based language, rather than having a visual drag and drop interface like Scratch. This doesn't mean that it can't be used to create graphs, or graphical user interfaces (GUIs), or even web interfaces. It just means that we write it as text.

One way of creating solutions to problems with programming languages is by creating a model of a problem so it is easier to understand. Since Python is an object-orientated programming language, it can be used to create custom data objects that more closely model our solution. This makes it easier to describe real things when programming.

For example, say we wanted to create a way to keep track of books in a library. We can use Python to represent books and the different attibutes a book has. Examples of book attributes could be:
 - number of pages
 - fiction or non-fiction
 - category e.g. history, art, biographical, science fiction, thriller etc.
 - hardcover, paperback, or ebook
 - ebook formats available

So we could create a book object in Python. And a book object could have a number of actions performed on it. In object-orientated languages, these are known as `methods`. We could also have a base book object, and then have other book objects that are based on the original book object. This means they are still books, but with additional attributes. e.g. an ebook is still a book, but can come in a number of formats. So we can group these book objects and their methods (actions that can be performed on them, or things they can do) as what is called a `class`. This is as much object-orientated talk as I want to go into here though.

I've tried to explain this in fairly simple terms, since the idea is only to show that Python is a much bigger, and more powerful, langauge than Scratch. We can still use the ideas we learned about in Scratch, such as decision making, input and output of data, repeating tasks, and keeping data in a variety of structures, such as lists. In addition to this, I've already talked about some of what Python can do in another post. And believe it or not, doing complicated things in Python can sometimes only take a few lines of code!

## HTML and web interfaces

By starting with Scratch, we learn simple programming ideas such as performing a number of tasks, and making decisions based on information provided to our program. Then we can use these concepts to step up to Python programming, which just happens to run on multiple operating systems, and can interact with many more things such as computer networks, files, devices, and so on. Although Python is text-based, (we have to type a bit), the more things we create in Python, the less we have to create because we can make our code *reusable*.

We learn about HTML and create web sites in Code Club because later we can access a web interface with mobile devices, and our laptops. What this means to us, is that we can create a web application by combining our Python code with HTML to let our end-users do cool things. Last year we went through some examples of web sites that run on Python. In a similar way that Scratch is an easier way to approach learning programming, Python is an easier way to start writing very capable programming. Although there are many programming languages, it's quicker to start making something happen in Python whereas other programming languages can require a lot of code that won't make sense. So Python is much more minimal, which makes it easier to learn with. Another language that is also like this, is Swift; used for creating applications on Apple devices.

## Are we going to make mobile apps with Python?

A few people at Code Club asked whether we can use Python to create a mobile app. The answer to this question is 'no' (technically you can but it's not really the best-suited language for it) but with Python we are more likely to create a web application rather than a native (runs on the mobile device) app. As I mentioned above, a language like Swift would be more suited for creating a mobile app. Stencyl is a visual environment suited for games, and the programming interface does work a lot like Scratch. A couple of main differences between Scratch and Stencyl is that Stencyl has a lot more features, and the resulting games can be run online in a browser, on a computer, and also on mobile devices. These can then be pushed to app stores and some very successful games have been created with Stencyl.

There are however, computer tools written in Python, such as editors, bug tracking systems, and even security tools, and much more.

## I don't want to type, and what about these ways of creating without any programming?

The main objective of Code Club, is to teach programming skills so that you have the best way to go from an idea, to something that is really useful. One of the objectives is to help you become familiar with programming concepts and fluent in some programming languages. Some of the advantages of this are:

- if you wanted to automate a task that takes a long time every day, you could do this and save yourself lots of time in the long term
- you can add your own ideas to other peoples' ideas by collaborating
- you can connect devices together to create new inventions
- you can build tools to make existing technology do more than they were intended to do

For example; although we use the Tickle app to control drones and Spheros, using modules available in Python we could write code that uses a Sphero as an interface to control a drone, or make a tool to automatically modify 3d printer designs in a way that the current software won't let us, or we could program a tiny computer to be carried by a drone and perform tasks with sensors that it was not rpreviously equipped with. We could even create a tool to help us understand how the current applications are interacting with our devices, and improve or adapt these to other uses.

## I want to create something, but I'm not sure how

That's great! A good way to get started is to look at other peoples' code and try to understand how it works. Then think about how you might be able to apply that to your program. Try to break down what you want to do, into smaller tasks. If you say, wanted to make a platform game, try breaking your idea down into the various parts, for example:

 - moving a player's character around the screen using key controls
 - creating gravity
 - preventing the player from falling through objects that should be solid
 - keeping score
 - prevent the player from disappearing off the side of the screen

 Keep asking the teachers and volunteers at Code Club, until you get the information you need. Sometimes it may be as simple as pointing you in the direction of some information that is online. There's plenty of tutorials too, and sometimes it just helps to see a simpler example to figure it out in your head. If a friend is doing something cool, go and tell them, and either look at their code or ask how they got it working or figured it out. Hearing about someone else's thought processes or workflow can be useful to improve how you approach solving problems, or troubleshooting a bug in your code. If you look something up and it doesn't make sense, just find another example of the same thing, or ask someone to explain it to you. It's always useful to try and walk through lines of code and predict what will happen before running it.

And if things just don't work, don't be afraid to make a copy of your own work, and then go right back to the start. If you have a plan sketched out, that can be invaluable to keep things simple and clear in your mind. Perhaps you find it harder to concentrate when there's lots of noise during Code Club: We have allocated some quiet areas for our Code Club, and the feedback we get is that some people find it easier to focus on what they are working on. At times it can also make the time seem to pass quite fast. This usually means you're working hard and will likely make some good progress. Other times, walking away for 10 minutes can give you a new perspective and help to re-focus.

Don't forget that you'll progress faster if you do some programming each day, even if it is just 10 minutes each night at home. Make these skills your own first and foremost, rather than thinking of it as a set task, or work to be done. If you treat Code Club as an opportunity, you'll get more out of it.
