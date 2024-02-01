+++
title = "Setting up robots for Code Club"
date = "2016-04-20T23:35:00Z"
tags = ['robots', 'raspberrypi', 'python', 'scratch']
description = "Last year we put together some robots, using a couple of Raspberry Pi 1B computers"
+++


I thought it'd be interesting for our Code Club kids to see behind-the-scenes, and for other Code Club teachers/volunteers to see our process. Firstly, there's some really good [information provided by Dexter Industries](http://www.dexterindustries.com/gopigo-tutorials-documentation/), who make these robots. I've pulled this post together from notes made at the time.

This post covers the first few steps I went through last year, setting up the GoPiGo robot. Since we have done a bit more Python this year, the aim will be to program this with Python, and our BrickPi robot will be programmed in the older offline version 1.4 Scratch.

Both these robots are each driven by a Raspberry Pi 1B computer, connected to Dexter Industries boards. We use 12volt battery packs to power these as well as motors and sensors. I'd recommend having them plugged in when programming, since it prevents the batteries from being used as much.

One issue I had with the BrickPi out of the box, was that the power connector for the BrickPi board was connected with reversed polarity. This was obvious when the batteries became really hot as soon as they were connected. Quickly disconnecting the battery pack, I checked the documentation and once I had corrected the polarity, everything operated correctly.

Anyway I'm getting ahead of myself. Last year we bought a BrickPi board to control our existing Lego EV3 motors with Scratch and Python. The grade 6 kids were divided into teams for a number of robot workshops. In this era of many distractions, a simple [inforgraphic](https://infograph.venngage.com/p/60410/brickpi-scratch-and-python-infographic) was a good way to show a high-level idea of how it all sits together with the BrickPi.

An issue with setting up VNC at the time was fixed using [this](https://www.raspberrypi.org/forums/viewtopic.php?f=66&t=12993). Since then, Dexter Industries have implemented an [easier way to connect](http://www.dexterindustries.com/raspbian-for-robots-update/) to the BrickPi and GoPiGo via the browser.

For the workshops, we started by looking at the example Scratch code that comes with the Dexter Industries robot operating system (robotOS; a modded version of Raspbian). From this, we would discover what 'broadcasts' need to be sent from Scratch to the Python script in order to:

 - move forward and back
 - turn left and right using a few different methods
 - stop and start

One script that comes with robotOS is the 'car' script, which allows the robot to be controlled from the keyboard. Since our BrickPi motors are mounted upside-down for a lower centre of gravity, the first task was usually to correct the forward and backward controls. Lessons we'd learned with Scratch activities come in handy when we look at replacing the interactive controls to use a script to control them.

Once we got to this stage, we needed to read data from the EV3 sensors. This was a bit of a problem as we were never able to get the sensors working properly. Over the holidays, I looked into this and found that we needed a firmware upgrade for the BrickPi to use the EV3 sensors. Again, a script on robotOS assisted with checking the firmware version. After successfully doing the firmware upgrade on the BrickPi, it became apparent that the Python script, that listened to our Scratch broadcasts, was only sending the commands for the older Lego Mindstorms motors. Looking further into this, I found the required commands in some other example scripts on robotOS, and added these to an modded version of the original Python script.

Since I've been pulling this together from my notes, I'm gradually adding to this post as I go. As other Code Club volunteers and STEM teachers can probably attest to, it is not uncommon to get something working the night before a session, and updating documentation at odd hours. Take this as a rather live blog in that sense...
