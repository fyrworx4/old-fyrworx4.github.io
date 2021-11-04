---
layout: post
title: 	"Docker Demon"
date: 2021-09-24
tags: [blog, docker]
---
It all started with creating a networking workshop for the school's cybersecurity organization that I'm currently leading as president. My team and I wanted to stray away from the conventional method of teaching -- lectures, presentations, bullet points on slides.

One of the main goals of this year is to provide very practical and tactical knowledge that members can take away after attending our meetings and workshops, and we wanted to do something pretty insane. And our mind turned into some sort of networking scavenger hunt.

## The Issue with Networking

We wanted to do something similar to teach members the practical commands and techniques to practice networking. The issue is that there's not many good resources to learn about networking as a beginner.

There are a plethora of terms, definitions, and concepts that you'd need to understand to make sense out of networking, and it's impossible to cover all of those topics within a two-hour time period, so we needed to think of something else.

## OverTheWire Inspirations

If you haven't heard of OverTheWire games, OverTheWire provides a public-facing server where you can solve puzzles to get to the next level. To get to Level 1, you'd have to SSH into this public-facing SSH server as a user called "level1", and you'll find clues in that user's home directory to get to the next level, which is the user called "level2".

I'm a pretty big fan of the Pareto principle, or the 80-20 rule, which shows that 80% of the consequences come from 20% of the causes. If we apply this principle to something like learning Linux, 20% of what you learn in a Linux is 80% of what you actually *need* to do on a daily basis. Commands like `ls`, `cd`, and `cat` make up an insanely miniscule portion of Linux, yet, in practice, are probably the most widely used commands that you use in Linux.

OverTheWire does an excellent job with teaching that 20% of what you need to know in Linux to achieve 80% of what Linux offers. But how do we do that with networking?