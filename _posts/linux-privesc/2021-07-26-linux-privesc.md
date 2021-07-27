---
layout: post
title: 	"Linux Privilege Escalation"
date: 2021-07-26
tags: [cybersecurity, penetration testing]
---
## Linux Privilege Escalation

TLDR: I didn't know Linux can be so overpowered when misconfigured.

Recently, I had the opportunity to experiment with privilege escalation techniques on Linux using [TryHackMe](https://tryhackme.com). For those that do not know, TryHackMe is an online platform designed to build small labs to hone in on specific skills in security. Although I have owned a few boxes on HackTheBox, the techniques after getting initial access into a machine still remained a mystery to me.

Until the Linux PrivEsc course.

This course is designed to walk you through a variety of Linux privilege escalation techniques, which one of them had me absolutely floored and probably made me consider being a Linux main for my CCDC team.

Here it is... shell escape sequences.

#### shell escape sequences

I had no idea that these types of methods even existed. Who would have thought that the simple `find` command could be used to break out of a non-sudo user?

By the way, in order to use `find` to get a root shell, you first need to make sure that your current user is able to run `find` with sudo privileges using:

```bash
sudo -l
```

And if `find` is within the list of privileged commands, then executing this command will give you a root shell:

```bash
find . -exec /bin/sh \; -quit
```

But there's more. There's this whole list of legitimate commands in Linux that can be used to do crazy things. It's [here](https://gtfobins.github.io).

#### overall experience

This made me even more hyped about penetration testing, which I had never considered as a career but was always curious about.

These topics seem so simple, yet so overpowered as an attacker.

Really fun way to learn more about Linux PrivEsc but also how to secure against these misconfigurations. And about Linux in general.