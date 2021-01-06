---
layout: post
title:      "System Design - Part 4"
date:       2021-01-06 18:25:50 +0000
permalink:  system_design_-_part_4
---


* A hosting service vs a web server
* A content delivery network and why it is important in large scale applications
* A load balancer and why it is important in large scale applications
* How many reads and writes your application makes and how that would change as it scales
* What the differences are between types of databases

Last time we spent some time talking about how to build out the beginnings of a scalable application when while working with things like load balancers.  This week I'd like to talk about how the actual requests that are made to a server you are working with dramatically impacts the performance of an application.

Think for example that you make a post request when a user logs in, and the user then makes a get request to pull data for a piece of information that gets rendered on their page.  1 post, and 1 get doesn't seem that bad, yet.

The problem is that as you scale users that 1 post and 1 get turns into 1 million of each.  This can keep scaling dramatically as you continue to add features to your application.  Think about it like this.  If you have a twitter feed where you pull in information from a feed, thats going to be at minimum one get.  But lets say you like a post and reshare it.  That may be two more gets and a post.  

As you can see, the number of gets and posts can get astronomical per user as the product scales.

This is a serious problem and can create serious bottlenecks for applications.  One of the best ways to deal with this is to have things like a load balancer, Content Delivery Network and the usage of a large cloud service like AWS or GCS on your side.

Thanks, 
Gabriel Joseph
