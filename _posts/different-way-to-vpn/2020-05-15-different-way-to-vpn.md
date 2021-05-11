---
layout: post
title: 	"A Different Way to VPN (through AWS)"
date: 2020-05-15
tags: [cybersecurity, vpn, networking]
---
Although we currently live in these unexpected times, it’s important for things like work, school, and other projects to continue, which brings an importance to having good “work-from-home” policies as well as secure access to company networks in order to access important files. This can be done through hosting a VPN on the remote network, but there are times where you won’t be able to access devices like routers to ensure that you’re correctly forwarding traffic.

Just kidding. This isn't about the importance of having a secure VPN.

This is about using a technique called NAT-holepunching to expose certain ports on an internal server.

And that’s where AWS comes into play.

By setting up a public-facing AWS instance, and a reverse SSH tunnel between your VPN server and the AWS instance, you will be able to successfully create a remote-site VPN connection.

Here is the [link to the guide][link-to-guide].

[link-to-guide]: https://github.com/fyrworx4/pritunl-reverse-ssh-tunnel-to-aws