+++
title = "Helping beginners learn to troubleshoot their code"
date = "2016-09-29T09:15:00Z"
tags = ['scratch', 'python']
description = "While learning to code there's a point where the student finds that the code they've written doesn't work.."
+++


After the initial excitement of 'hey I'm actually coding!' and creating some working code, the next step is often to put together the code in different ways and test our understanding. The faster you progress, the sooner this time will come. In other words, having your code not work is a great sign that you're putting in the effort to progress. This also applies if you're a teacher or volunteer who may be starting to put things together yourself,  while helping kids learn. It always helps to have a positive approach when helping someone who has reached this point for the first time i.e. it's a good thing, and a great opportunity to learn!

![screenshot](/images/doesnt_work.png)

## Find out what we are trying to do
The first thing to ask when helping someone, is to find out what they are trying to do with the non-working code. Have the student describe the idea behind the code. If things are unclear, ask about the context of the code in the game or program e.g. 'Tell me about the overall idea of the game'

## Have things become over-complicated?
Before we walk through the code, it's important to ask ourselves whether we're using the most straight-forward approach. Sometimes things can become more complicated than they need to be, without us even realising. Taking things back to basics can make the code seem clearer and easier to read, especially later on. Once we know what we are trying to achieve with the code, we can work out whether it is the simplest and most readable way to do it.

## Strip the code down to the bare basics
If you find that the code has become overly complicated, it can help to take out some of the extra code. In Scratch, you can leave these in the scripts area, as they won't run unless there is a starting block at the top, such as `when green flag pressed`. This can make it easier to replace the code if we need to. Other times, it may be possible to create a fresh project; in another tab, if you're using Scratch online, or in another file if we're using Python. Keep in mind, with Python, you can also try commands out in the Python shell using [interactive mode](https://docs.python.org/3/tutorial/interpreter.html). Once you've solved the problem in the code, you can easily add the other parts of the code, if they are still required once it is fixed.

## Talk through your troubleshooting thought process
When I was learning to code as a kid, I still recall someone trying to help, almost silently whispering to themself, and it felt bad to even ask what they were doing. I found it hard to know what they were doing, and would have to ask them to explain it afterwards, which sometimes ended up seeming more complicated than it should have been. While helping someone troubleshoot their code, it really helps to talk about the steps you're going through. The first step might be to walk through the code, line by line, and asking questions about the code like, 'What does this do?' or 'Is this the section that checks whether the player has died?'. Asking questions like these can also help the student or yourself understand their code better, which may help solve the problem. Talking through the steps you take to understand the code, can also be useful. This could include, 'Ok, so we're checking whether our sprite is left of this positing, is that what we want?' or 'It looks like we're only checking once to see if a key is pressed, should we be repeating this forever?'. Usually, going through these steps can get the student to suddenly realise what the problem is, and also learn how they would approach a problem next time. The idea is to also show the student how to approach troubleshooting, in addition to fixing the immediate problem with their code.

## Reinforce what we learned while troubleshooting
Once the problem with the code has been fixed, and everything is working, it helps to quickly summarise what was wrong. The student will be keen to get on with things at this point, so keep it quick and clear. e.g. 'It looks like we needed to check for a keypress all the time, rather than just once'. Then talk about how we could prevent these problems again, 'So just remember when we checking for keys to be pressed using `if..then` we can put it in a loop to make it repeat`.

## Start simply
Sometimes the project could turn out to be overly difficult for the student. If there's some things that the student might need to learn first, it can help to take them back to a project that helps them understand the concepts before tackling a more difficult project. Most students will find this easier as it allows them to make more progress and feel less frustrated. 

