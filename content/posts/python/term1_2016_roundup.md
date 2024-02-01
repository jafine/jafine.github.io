+++
title = "Term 1 Python roundup"
date = "2016-03-30T22:30:00Z"
tags = ['python']
description = "Concepts we covered"
+++

In term 1, grade 6 people who were in Code Club last year, went through some Python concepts.

The activities we had a go at were:

  1. Using a text editor e.g. notepad, in Windows, we went through the *inventwithpython* [guess the number](http://inventwithpython.com/chapter4.html) exercise. We discovered that the Macbooks' Windows defaulted to Python 2, which we later fixed by running our scripts from the cmd prompt using:  
        `py -3 <ourfile.py>`.  
Some people had a go at copying and pasting the code and soon found out that this changed formatting as well as copying the line numbers. In some ways, this was more work because line numbers had to be taken out, indenting had to be restored, and carriage returns needed to be re-added. Our Python coding (development) environment at this stage consists of:
    - A Python shell that allows us to type in interactive Python commands, to see how things work before putting commands into a script. Later this was especially useful when using the Python turtle module.
    - A text editor. We used text editors because, previously, we'd had varying success with IDLE and Tinker. It was a little confusing to easily see the difference between the editor and shell when loading scripts in IDLE. In Windows we used notepad because it's already there, in OSX we used nano from the terminal. Nano was useful when we later connected to the Raspberry Pi using ssh to build things with Python Minecraft Pi module functions. This is also useful since we also have some robots that we run with model 1B Raspberry Pis.
    - A command shell/window. We ran out scripts after running cmd.exe to get a command window. Later we found that it was easier to just save our scripts, but keep them in the editor, so that we could easily make changes to fix errors or add different code.   
                
  2. Code Club turtle activities.  
This time we discovered that the netbooks running Windows did not have Python3 at all. So we ended up trying to do things in the Python shell, but it was a frustrating session. A few of us ran some of the turtle scripts, which didn't need Python3. The initial idea of this session was to build on the previous 'guess the number' activity by adding loops and introducing the concepts of:
    - Don't repeat yourself(DRY). This means trying to write efficient code, using structures such as loops, to repeat the same commands.
    - Functions. This is part of DRY.
    - Troubleshooting errors. I think we needed to get started quicker. This worked better in the next session.  
         
  3. Continued Code Club Turtle activities.  
We were one teacher down for this one in the later part of the session. Things worked better because we sat on a round table and I think it was easier to talk to everyone to get things working. I think we all got multiple stars drawing this time, with some people opting to use OSX, which was easier. Some things we looked at were:  
    - The basic idea that we our scripts are starting to have:
        - An initialistion section. We set up things like variables here. This was easy to remember by talking about what happens when we don't reset our score when re-running a Scratch game.
        - Function definitions.
        - Main, which usually contains our commands or main loop that controls everything, and where we call functions we created.  
    - Functions. We looked at the ideas of:
        - Built-in functions that come with Python
        - Functions that we can import from modules
        - User-defined functions that we define ourselves.
        - Adding parameters to change how our user-defined functions work.  
An example of how we define our own Python function could be:  

                :::python
                def star():
                    for i in range(6):
                        forward(100)
                        right(120)
  
        Then this would give us a `star()` command that we could use to draw a star without typing all those lines. Later we looked at adding parameters so we could tell the function how big, or what colour to draw the star with. At a later stage we'll look at functions that can 'return' information to us when called.

  4. Using a Raspberry Pi computer and connecting with ssh and the OSX terminal, we examined, ran, and edited Python scripts to try and build a building in Minecraft Pi.
