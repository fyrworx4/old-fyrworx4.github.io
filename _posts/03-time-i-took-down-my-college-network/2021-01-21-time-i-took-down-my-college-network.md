---
layout: post
title: 	"The Time I Took Down My College Network"
date: 2021-01-21
tags: [networking]
---
I love computer networking. In fact, in my CCDC team, I opted to be the networking lead and became the de-facto person in my cybersecurity organization to talk about computer networking.

It’s more of a love-hate relationship. Networking is super interesting to me, but even a few small changes can bring down an entire network.

And I’m notorious for bringing down networks. It’s how my role in CCDC became nicknamed the “not-working” team. There would be many times where I accidently applied an ACL (access control list) that would block a scoring service from reaching outside the network, bringing us down for a few hours until someone realizes that it’s a networking problem.

Despite that, I’m still the go-to person for any networking needs.

This past summer, I had the opportunity to redo some of the networking infrastructure for my school, specifically a small lab designed for cybersecurity labs, class demonstrations, etc. It’s called the Student Data Center.

I assisted with planning out and pushing for a networking configuration that would give us the most bandwidth, while at the same time, have redundancy all over the place. Redundant links, switches, and more. The problem was that there wasn’t enough documentation for me to understand how the networking was setup before, so there was no way of telling if there were devices that were owned by the school, or owned by the Student Data Center.

One day at the lab, there were a few Cisco switches that bridged our lab to the main campus network, and I wanted to see the configuration of those switches, but didn’t know the passwords to them. There wasn’t any documentation on any of the switches, so *wouldn’t it be a great idea to flex my Cisco knowledge and do a password reset on the switches?*

So I did.

Long story short, it didn't go well.

For some reason, after my first password reset, the commands of the previous configuration were all being automatically inputted into the switch, and some of them were generating errors. I had no idea what was going on, so I just continued on and saw if I could do a show run on the switch.

And I didn’t see any of the previous configuration.

I might have accidently wiped the switches and brought down the entire lab network.

To make matters even worse, the Cisco switches were school property, meaning that what I did was technically unauthorized.

I can’t help but feel to this day that this was entirely my fault, that I should have communicated more clearly which devices were in scope for this project, but at the same time, I’m glad that I did it in a lab environment, where there is a lot more room for failure than something like a business.

Lesson learned - always ask before doing something.