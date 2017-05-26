---
layout: post
title: "10x more free space"
date:   2017-03-26 17:00:00 -0600
categories: blog
---

Effective immediately, we are increasing the amount of free space on Neocities for all users to **1GB**, a 10x increase over the previous limit (100MB). Supporter free space will also be doubling, from **10GB** to **20GB**.

This increase is thanks to the launch of our new [Ceph](https://ceph.com/) based storage cluster, which we've designed to scale and be cost effective in the long term, while still providing the reliability, durability, and performance the modern web comes to expect.

In addition to providing enormous storage capacity for future growth, our serving infrastructure is now completely redundant in the event of equipment failure. If any networking equipment or servers go down, a backup automatically kicks in, allowing Neocities sites to continue being served and updated even if 2/3rds of our servers go down, or if we lose half of our upstream internet connections.

With this launch, and our recently deployed 11-datacenter global anycast caching CDN, Neocities becomes a world-class web hosting service, proving you can still make building a web site fun and easy without sacrificing performance, and without being forced to figure out how to use esoteric, expensive cloud services.

We'll be doing some deep dives into our new infrastructure in the future, including discussing how we built our own [anycast network](https://en.wikipedia.org/wiki/Anycast), and how careful design allowed us to reduce our bandwidth costs by 18x compared to the leading cloud and hosting providers. Stay tuned for that.

These upgrades were made possible by our [supporters](https://neocities.org/supporter): Thank you!

More space, more speed. What are you waiting for? [Make your own web site now!](https://neocities.org)
