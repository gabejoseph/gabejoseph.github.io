---
layout: post
title:      "System Design - Part 2"
date:       2020-12-23 15:46:42 +0000
permalink:  system_design_-_part_2
---


Last time I spoke about the overall nature of system design and how it is something that is critical to understanding how applications work.  I listed the following as things I would be focusing on as well.

* A hosting service vs a web server
* A content delivery network and why it is important in large scale applications
* A load balancer and why it is important in large scale applications
* How many reads and writes your application makes and how that would change as it scales
* What the differences are between types of databases

This week we will be spending time on the differences between different databases.

The two databases I wanted to mention are SQL and NoSQL databases.  There are several key differences between the two and they each impact what kind of db you should use in building and then ultimately scaling your application.


1.  SQL databases are relational.  This means that there are things like keys that are passed between the different models you are working with and because of this there are established relationships that develop.  NoSQL isn't like this, the information is non-relational and can be better in certain applications. 
2.  NoSQL databases are more unstructured.  In SQL databases the information is clearly outlined, and things can be queried.  NoSQL has a much more dynamic organization which allows for more unstructured infomation.
3.  Scale - NoSQL databases can be scaled horizontally by processes called sharding or a p2p network.  This allows for a large and vast horizontally scaled network.  SQL can be scaled vertically, which means that you can create more and more complexity on a single server.  Ultimately NoSQL is better for large sprawling systems.
4.  SQL databases are table based, while NoSQL databases can have various ways of storing information.  
5.  SQL databases are good for multi-row transactions while NoSQL is better for things like JSON objects.

And there you have it!  

Happy Holidays!


