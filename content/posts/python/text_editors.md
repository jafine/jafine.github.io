+++
title = "Text editors and helping kids learn Python"
date = "2016-05-15T14:24:00Z"
description = "In our Code Club we have Windows, Mac OS X, and Linux, so we've had some success using whatever editors we can to edit Python scripts.."
+++


This post is primarily about some of the discussions we've had about facillitating Python coding at our Code Club, some of our experiences as a Code Club, and some of my ideas about what the kids can use Python skills for.

Dealing with a variety of different operating systems for a variety of different projects, I try to use whatever tools are available on the platform we're using, and do the job. Although it might take a little bit longer to get the hang of things, and sometimes it's not all as straightforward as we'd like, it means we end up being a little more adaptable. We purposely use tools that are free and open source, or that come with the operating system, whenever we can. e.g. there's been times when we've just use notepad on Windows, or nano in a Mac OS X terminal, or when connected to a Raspberry Pi. This gives more flexibility since we can add our own modifications if required, and makes them readily accessible for kids to be able to replicate things at home. I think that is really in the spirit of learning to make our own code creations, and contributing to improve things as we go. Also, when we initially used the Python IDLE tools, the kids were getting a bit confused, until we were able to explain that Python scripts are really just text files.

We played with Tinker for a short while, although for it seemed like it abstracted Python and HTML away from being able to interact with real things. Some kids seemed frustrated that they couldn't easily upload their own image files, and we couldn't import other Python packages. Since we've already talked about web sites, applications, and robots that use Python, it makes sense for us to be using Python in a context where this seems more accessible.

Likewise, although sometimes we will start looking at devices like the Sphero, that are initially controlled with an app, I've had some great discussions about what's really happening behind the scenes. Once we understand how things really work at a low level, it's great to try and write some code that will allows us to control things directly. I remember a friend at school once saying that while coding sounds good, "it's all still just on a screen". Interestingly, that friend does spend a lot of his work time sitting in front of such a screen. The really exciting thing about having Raspberry Pis connected to arduinos controlling robots, is that suddenly not just stuck in a computer screen, we're affecting the world around us. One of our students last year mentioned that he had initially thought coding was only about games, and during Code Club, had realised that it meant he could make all manner of useful inventions that were driven by code.

Some issues we come across when using a variety of editors include:

 - sometimes the lack of line numbers can make us work a little harder to troubleshoot our scripts
 - we have to understand the basics of how to get around without a mouse at times
 - linefeeds in a file taken from one operating system can look like rubbish in the editor of another operating system
 - we get less information while typing in our code
 - the more basic editors don't recognise that we're writing Python, so they don't highlight important parts of the commands (syntax highlighting) so we actually have to know what we're doing...eventually

I'd forgotten the Atom editor until recently. I used to use it just for HTML and style sheets, but then I remembered it can work nicely with Python, since it recognises it and fixes most of the above issues (we'd still need nano in a terminal). However it is supported across Windows, Mac OS X, and Linux (not so much on the Raspberry Pi at this stage). It is also really easy to install, by just grabbing a `.dmg` file for Mac OS X or an installer for Windows, and so on. This possibly makes it a lot easier for Code Club teachers and volunteers to install on their own systems. Although I suspect that there will be some point where we will need to show how to install `pip` and grab the Python packages we need. 

You can install the Atom editor by following the instructions [here](https://atom.io/) for your operating system e.g. Windows, Mac OS X, or Linux.

![screenshot](/images/editor.png)
