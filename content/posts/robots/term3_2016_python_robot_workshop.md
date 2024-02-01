+++
title = "Term 3 Python Robot roundup"
date = "2016-09-12T23:00:00Z"
tags = ['python', 'robots']
description = "Looking back at term 3"
+++


This term we had some great fun with Python.

## Raspberry Pi Robots with Python
One of the major changes was the introduction of a second robot workshop, using the GoPiGo by Dexter Industries. One of the key differences in this robot, from our BrickPi robot, is that it doesn't use Lego Mindstorm parts. It is equipped with a camera and ultrasonic (distance) sensor, which can be rotated together in an arc, using a small servo motor. Last year, our Scratch robot workshop was run with larger groups of around five students. But there just wasn't enough for everyone to do at once, which left some idle or distracted. This year we ran both robot workshops with teams of two; one person to monitor the robot, and prevent crashes, and the other writing and runing the code. These roles were often swapped beteen the pair, during the activity. We found it great to use Python for the GoPiGo, as it took Python away from being only on the screen, to something that could make phyiscal things move and react. It also helped show that the skills, we learned in earlier activities, helped us to feel comfortable in different programming environments. Hopefully, the extra flexibility we get by using Python will allow us to take some of the ideas the kids have, further in the future.

![screenshot](/images/gopigo_in_action.png)

## Useful skills
Some of the skills we learned earlier on were  useful when programming the Robot in Python. These include:

 - using the Python shell to try out commands and figure out bugs in our code
 - understanding different ways to edit Python files in Windows, MacOS, and Linux
 - learning ways to view files while editing others
 - using the command line for moving around the file system, and listing files or directories

## The GoPiGo workshop`
With some of the grade 6s, we have been going through learning about some networking and connecting to a command terminal on the Raspberry Pi in the GoPiGo robot. By examining Python files, we were able to see where functions were defined. Looking at the example Python files, we could see these importing the functions from the other files, to make it easier to write our programs. During a quick demo we sa the difference between import with `import <module>` and `from <module> import..` and talked about the confusion if we were to overwrite our built-in functions such as `print()` in Python. Going through the Dexter Industries example Python files line-by-line enabled the kids to put together their own scripts rather than copying and pasting. So by taking a very different path to making our robot autonomous, compared to the BrickPi robot workshop, the kids ended up feeling much more confident with Python. There's been a lot of questions that begin with, "In Python, can we...".

## Improvements in our lab environment
One of the main roadblocks in our Code Club, has been a lack of control in software and network access. For the robot workshops, we started using a home-made wifi router, that I built from a Raspberry Pi Zero. Although this worked very well for our field trip to demo our kids' skills to politicians, we started to have issues back at school. Eventually, I got a cheap TP-LINK mobile wifi access point (which runs open source software -  woohoo), resulting in better productivity in our robot workshops. We've also ended up starting the robot workshops as soon as the kids arrive, so we get the most value from the time. We ran both the BrickPi and GoPiGo robot workshops in an area that was partially separated from the main Code Club activities. This allowed kids to stay more focussed, as it was part of the quiet area that we have set up. It was also really useful to have a whiteboard or similar to quickly explain concepts; so we could just get on with the 'doing' part of the workshop.

![screenshot](/images/router.png)

Some other things to consider with a lab environment would include what sort of networks you are allowed to expose the computers to, and what sort of access is required for a given activity. Generally, there should be no need to ever have the computers directly Internet-facing i.e. with an IP address that can directly be accessed *from* the Internet. If you want to use some of the new Google resources for speech and image recognition, you'll only need to initiate connections out to the Internet, rather than from it.

## Moving forward
Now that we can comfortably connect to the robot, and write some useful Python, it will be exciting to push ourselves further, using the picamera, sensors, and a handy little amplified speaker we found. One idea was to get the robot sending some information to a Raspberry Pi web server we have set up! 
