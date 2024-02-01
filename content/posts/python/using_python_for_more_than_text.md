+++
title = "Importing more Python functionality"
date = "2016-05-19T20:41:00Z"
tags = ['python']
description = "When you first print something on the screen with Python, there's usually a spike of excitement, however this can wane when progressing on to other mostly text-based exercises.."
+++


## Python built-in functions and modules

At Code Club our first Python scripts usually involve using built-in commands, otherwise known as functions e.g. `print()`, `input()`, `int()`. A list of built-in functions for Python 3 is available [here](https://docs.python.org/3.3/library/functions.html).

Sooner or later we might want to do something a little more interesting, like generate some random-ish numbers, or process some information in file, or connect to another computer. In some of the Python tutorials we've done, you'll notice the `import` statement being used to import more functions from the the [Python standard library](https://docs.python.org/3/library/).

An example of importing from the Python standard library:

```
import random

random_number = random.randint(1,1000)

print("Here's a random number: ", random_number)
```

You could type the above Python code directly into the Python 3 shell or put it in a text file and called it something like `print_random_number.py`.

We could run the latter in the Mac OS X `terminal`, in Linux e.g. on a Raspberry Pi, or in the Windows `cmd.exe`.

To run it in Mac OS X, type:

```
python -3 print_random_number.py
```

Which results in:

```
Here's a random number:  716
```

We imported the module, `random`, from the Python standard library. To run the function `randint()` from this module, we put the name of the module in front of it. This particular example will generate a random-ish (pseudo-random) whole number between 1 and 1000.

If you looked at the [Python standard library](https://docs.python.org/3/library/), you'll have seen lots of things to import for your Python scripts.

Sometimes when we start learning to code, other people who can already code get excited and really want to tell you all of the cool stuff you can do. But if they did that, it could easily be overwhelming and make it look too way too complicated and hard to learn. But once you get a few scripts written and start to think of problems that could easily be solved by writing a script e.g. reading information from a website, processing it, and adding it to a spreadsheet.

So...taking this import idea further, since Python is [open source software](http://www.opensource.org), anyone who is interested in learning, can contribute additonal functionality to Python.

## What else can I do with Python?

You can find a list of additional Python packages [on this page](https://pypi.python.org/pypi). There's over 80,000 packages there, each containing functions that you can import into your scripts. Go to the 'list packages' link on the left to see all of them (be aware this can take a while to load). These packages can make it possible to useful tasks in only a few lines. This means that assuming your code is logically structured, you can create scripts that are much easier to read, and add to. This is important if you want collaborate with people, or have others use your code in their creations.

To install these packages, a good way is to use a tool called `pip` or `easy_install`. On Windows, Mac OS X, or Linux if you're already installed Python from https://python.org, you can just download [get-pip.py](https://bootstrap.pypa.io/get-pip.py) and [run it with Python](https://pip.pypa.io/en/stable/installing/) (it's just a Python script). Then you can just type `pip search` to find a package you want, and once you know the name of the package, type `pip install <put name of package here>`. Usually there are examples of how to use the package online. It's best to try the examples first, so you can get something that works, to help you learn to use the functions in your scripts.

There are also a large number of Python projects stored in open source respositories like GitHub and BitBucket just to name a couple. When developers (people who write code) want to collaborate and share their code, they will store it in these type of respositories. This makes it easy for others to [fork](https://help.github.com/articles/fork-a-repo/) their projects, and either contribute using [pull requests](https://help.github.com/articles/using-pull-requests/), or create a new project based on the forked project.

So if you have a gadget that you're using an app to control, it might be interesting to search online for a Python script or Software Development Kit (SDK) that you can use to control it with, and understand how you can integrate it into your own projects. Many of these scripts that can interact with interesting hardware, come about from interested people observing how something works, and then figure out how to make a language like Python, send the same commands. This can allow you more control and flexibility than the standard app controls, and allow you to trigger the controls using other sensors e.g. using a Sphero to control a robot. Sometimes what is happening inside the case of electronic hardware can be much simpler than we expect. But we don't know unless we try to listen to control communications or search for information that helps us. This attitude of curiosity is something I like to work toward at our Code Club.

Here's a video I found, by Paul McWhorter, showing how Python can be used to light up a Light Emitting Diode (LED) on a small Raspberry Pi computer.

<iframe width="560" height="315" src="https://www.youtube.com/embed/EM5gnNg7JTI" frameborder="0" allowfullscreen></iframe>

A few of the Code Club kids have installed Python at home. That's a good way to learn faster and more often, since it can be hard to learn quickly if you have to keep backtracking. Python is great because it's free and easy to write scripts without a lot of boilerplate code. Boilerplate code is lines of extra code that need to be added before you can start coding in some languages. It's nice that Python doesn't need too much of this, and because it recognises indentation, it's quite easy to see the structure of Python programs. This makes it a lot quicker to follow what is going on, and partially why we're starting with it. A really good exercise when learning to code, is to go through someone else's Python script and try to figure out what it does. Then if you get stuck, go and ask someone who knows a bit more, and get them to walk you through the parts that don't make sense to you.


