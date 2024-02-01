+++
title = "Micro:bit 2-way radio example"
date = "2016-12-21T16:24:00Z"
tags = ['python']
description = "With the micro-Python radio() function on the micro:bit, we can broadcast a emoticons to one or more micro:bits receiving on the same frequency.."
+++


![excuse for a drawing](/images/microbit_jafine_radio.JPG)

Lately I've been playing with the [BBC micro:bit](https://www.microbit.co.uk/). Having micro-Python on this cool device that boasts accelerometer, magenometer, bluetooth low energe (BLE), temperature sensors and a 25 LED matrix, and Integrated Circuit (I2C) interface makes it a easy entry point for kids to build and code on. So I was thinking it might be fun to send emoticons between two micro:bits, so here's a micro-Python script I put together to broadcast emoticons to other micro:bits running the same script. You'll need at least two micro:bits to send and receive emoticons, or if you have one micro:bit you can just use the A and B buttons to display different emoticons. For some reason, it's rather entertaining selecting emoticons to send back and forth through the air!

## Controls
Once the script is running on your micro:bit, it uses the following controls:

 - Button A: go to the previous emoticon
 - Button B: go to the next emoticon
 - Button A and B together: send the currently showing emoticon to other micro:bits running the script nearby

When you send an emoticon, the micro:bit will display 'sending...' and the receiving micro:bit will show a diamond, then display the received emoticon for 2 seconds. For this example, I've tried to stick to a fairly simple `if`..`elif` decision-making structure, using only the basics required to make this work.

## Let's get coding!
Ok, so let's get started...

First, open whatever editor you are using to write your code. Since we are using micro-Python, you can use:

 - the micro:bit [online Python editor](http://python.microbit.org/editor.html);
 - the [Mu editor](http://codewith.mu/); or
 - the [micro:bit plugin for Chrome](https://chrome.google.com/webstore/detail/micropython/lhdjeebhcalhgnbigbngiaglmladclbo?hl=en-GB), or any text editor with the [command-line `uflash` tool](https://github.com/ntoll/uflash).

In our editor let's begin writing the script and import the required micro:bit and [radio](http://microbit-micropython.readthedocs.io/en/latest/radio.html) modules. Add the following to a new file in your editor.

```python
from microbit import *
import radio
```

## Put the emoticons into a dictionary
The micro:bit's image class has built-in images that we can associate with numerical keys in a dictionary. We'll create a dictionary called `images`.

```python
images = {1:Image.HEART,2:Image.HEART_SMALL,3:Image.HAPPY,4:Image.SAD,5:Image.SURPRISED,6:Image.ANGRY,7:Image.ASLEEP,8:Image.BUTTERFLY,9:Image.DIAMOND,10:Image.CONFUSED,11:Image.COW,12:Image.PACMAN}
```

## Create an index
We'll use a variable to keep track of which emoticon image we have 'selected' and set this to 1.

```python
index_num = 1
```

## Configure and enable the radio
To set up the radio functionality we need to set the radio channel to 10 and turn the radio on.

```python
radio.config(channel=10)
radio.on()
```

## Main loop and receive radio data
Now we come to the main loop that keeps repeating while the script is running. Received radio communications will be captured in the `incoming` variable. To keep things simple I haven't done any validation on the incoming radio data. I'm just pointing out that you should be aware that this is reading unchecked radio data into a variable, and a rogue radio transmission could potentially exploit this. However, for the sake of this exercise, I'll assume you're well away from such transmissions and possibly in a Faraday cage or bunker of your choice ;)

```python
while True:
    incoming = radio.receive()
```

## Do things when events occur
The rest of the script is essentially saying "if something happens, do this" followed by displaying the select image and a delay. Without the delay, the micro:bit was checking the buttons too often, making it hard to read a single press. If you find that you have to hold down the buttons too long, you can reduce the `sleep()` delay value to make it a little quicker. If it flickers between different images when you press buttons, increase the delay.

Check for single button presses, and increase or decrease the `index_num` value. Since the if statements are inside the while loop, we need to make sure they are indented (moved right) so they line up with the `incoming` line above.

```python
   	if button_b.is_pressed():
        index_num += 1
    if button_a.is_pressed():
        index_num -= 1
```

Send the current `index_num` value, and display 'sending...', if button A and B are pressed together. The str() function converts the number into a character to send. We could really send raw bytes here but I'm trying to keep it simple for now.

```python
	if button_a.is_pressed() and button_b.is_pressed():
        radio.send(str(index_num))
        display.show('sending...')
```

If we have an incoming radio broadcast, display the `TARGET` image, wait for half a second, then convert the incoming data back to a number.

```python
	if incoming:
        display.show(Image.TARGET)
        sleep(500)
        display.show(images[int(incoming)])
        sleep(2000)
```

Make sure that `index_num` stays within the key values for the `images` dictionary. In this case, if `index_num` is too high, we set it back to the first image, and if it gets too low, we set it to the highest image.

```python
    if index_num > 12:
        index_num = 1
    elif index_num < 1:
        index_num = 12
```

Finally, display the currently selected image from `images` and wait for half a second.

```python
    display.show(images[index_num])
    sleep(500)
```

## The entire script
So the whole script should look like (I've added comments so don't worry about anything starting with `#`:
```python
# A micro:bit emoticon chat script
# By @justaboutfine
from microbit import *
import radio

# Create a dictonary of our emoticon images
images = {1:Image.HEART,2:Image.HEART_SMALL,3:Image.HAPPY,4:Image.SAD,5:Image.SURPRISED,6:Image.ANGRY,7:Image.ASLEEP,8:Image.BUTTERFLY,9:Image.DIAMOND,10:Image.CONFUSED,11:Image.COW,12:Image.PACMAN}
index_num = 1

# Set the radio channel to 10
radio.config(channel=10)
radio.on()

while True:
	# Capture received radio data
    incoming = radio.receive()

    if button_b.is_pressed():
        index_num += 1
    if button_a.is_pressed():
        index_num -= 1

	# Send the current emoticon if both buttons pressed together
    if button_a.is_pressed() and button_b.is_pressed():
        radio.send(str(index_num))
        display.show('sending...')

	# If there's incoming data, show the emoticon that's been received
    if incoming:
        display.show(Image.TARGET)
        sleep(500)
        display.show(images[int(incoming)])
        sleep(2000)

	# Keep the index_num within the valid dictionary key range
    if index_num > 12:
        index_num = 1
   	elif index_num < 1:
        index_num = 12
            
	# Show the current image
    display.show(images[index_num])
    	sleep(500)
```

Now flash this to two or more micro:bits and you should be able to use the controls listed above, to select and send emoticons from one micro:bit to another. On the Mu editor and Chrome plugin, you can just click on 'flash', with other editors you can compile your project to a `.hex` file and drag or copy it to your micro:bit once it is plugged in. Unfortunately, flashing via BLE doesn't work if you're using Python. Also, using radio in other languages can interfere with BLE functionality. If you have a group, you can send to more than one micro:bit. You can set separate radio channels on different pairs of micro:bits to have separate teams or emoticon conversations. From here, you could even use this to send text messages to one another as well, or use speech() to 'say' a message on another micro:bit equipped with a speaker. The possibilities are fairly broad, so go and experiment!
