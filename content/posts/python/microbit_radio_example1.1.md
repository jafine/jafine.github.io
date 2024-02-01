+++
title = "Micro:bit 2-way radio example - adding audio alerts"
date = "2017-03-13T09:40:00Z"
tags = ['python']
description = "With the previous Micro:bit 2-way radio example, we set up Micro:bits that talked to each other by sending data over radio. This is a quick post about adding some features to that code."
+++


This post adds onto the [previous tutorial](/python/microbit_radio_example1.md), so if you haven't already, you shoud go have a look at that first.

## Adding sound alerts
If you've got a speaker connected to your Micro:bit, or have the MI:Power battery add-on that includes a speaker, it's easy to add a sound to alert us of sending or receiving a new emoticon.

In the original code, we had an `if` statement that would display the TARGET image, pause, and then display whatever image the incoming index pointed to:

```python
    # If there's incoming data, show the emoticon that's been received
    if incoming:
        display.show(Image.TARGET)
        sleep(500)
        display.show(images[int(incoming)])
        sleep(2000)
```

Let's change that to play a couple of short notes, when we detect an incoming radio message. First we'll have to import the music functions for the Micro:bit. So, just after the existing `import radio` statement, at the top of the code, add the following import:

```python
import music
```

Now look for the `if incoming:` code and find the following two lines:

```python
        display.show(Image.TARGET)
        sleep(500)
```

To play two notes instead of displaying the target and waiting, modify the code as follows:


```python
    if incoming:
        music.play(["C4:2","D4:5"])
        #display.show(incoming)
        display.show(images[int(incoming)])
        sleep(
```

Save the Python code and send it to the Micro:bit. When it receives a message (emoticon), you'll hear it play the two notes and immediately display the emoticon sent.

The information for the notes are simply stored in a dictionary i.e. a list of pairs, known as tuples, in the format NOTE:DURATION. Because it's a dictionary, we put our NOTE:DURATION pairs inside square brackets, separated by commas.

Additionally, if you'd like to play some notes when sending an emoticon, you can find the line that checks for both buttons pressed:

```python
    if button_a.is_pressed() and button_b.is_pressed():
```

Now place a similar `music.play()` line after it. To make sure it's within the `if` statement, remember to indent it. Now when you write this code to the Micro:bit, you'll have sound alerts when you send and receive emoticons.

If those tones aren't to your liking, you can also use [speech.](https://microbit-micropython.readthedocs.io/en/latest/tutorials/speech.html)

For more information on creating sound on the Micro:bit you can find the documentation [here.](https://microbit-micropython.readthedocs.io/en/latest/tutorials/music.html#wolfgang-amadeus-microbit)

