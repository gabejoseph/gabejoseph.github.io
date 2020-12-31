---
layout: post
title:      "System Design - Part 3"
date:       2020-12-31 18:52:33 +0000
permalink:  system_design_-_part_3
---


* A hosting service vs a web server
* A content delivery network and why it is important in large scale applications
* A load balancer and why it is important in large scale applications
* How many reads and writes your application makes and how that would change as it scales
* What the differences are between types of databases

This week I'll be talking about load balancers.

As a company begins to scale and grow rapidly, a variety of different mechanisims are used to try and offset the tremendous amount of traffic that can get passed between backend servers and client devices.  Once of the most common of which is a load balancer.  Load balancers allow for the increase in concurrent or simultaneous users for an application.  This is a good example of something that allows for horizontal scaling of an application.

The load balancer distributes the massive number of requests that come in from clients and distributes them to servers that may be able to deal with those requests.  So in essenece, this mechanism seems simple, but plays a critical role as applications grow in size.

This also allows for more responsiveness of an application.  Think of the way games and videos would lag in the past.  As applications have grown to web scale, so has the technology behind distributing these requests.  This is why we deal with much more effective streaming, loading and uploading with large applications we use on a regular basis.

Next time I will touch on Content Delivery Networks as I explain the relationship between Read, Writes and Load Balancers.
