---
layout: post
title:      "Parler Hack "
date:       2021-01-15 13:01:33 +0000
permalink:  parler_hack
---


I thought this would be a great and relevant post that we could all learn from in building our future applications.  Parler is an application used by far right groups and was most notably was thought to be used to organize fringe extremists during the capitol building assault.  Well it was hacked by activists and massive amounts of data has been collected on the individuals who used the app.

*But how?*

Parler seems to be put together quite amateurishly, because there are three strategies that these hackers used to collect the information they would use.  An exposed API, unscrubbed EXIF data and incremental post id's instead of random ones.

API's are essentially any part of your pipeline that can be accessed through an endpoint.  Typically I'll have my backend structured as an API that has several endpoints that can be accessed to retrieve relevant data on whatever it is the frontend needs.  Parler seems to not have password protected their endpoints, leaving open a slew of private data which was up for grabs.  

Incremental post id's are another oddity that was left open for exploitation by hackers.  Apparently the post id's were not randomized, which meant that hackers could actually chronilogically sort posts and create a roadmap of what posts were created when.  This is important because it creates a standard amongst which other types of data can be linked.

Finally EXIF data is essentially metadata that gets linked to any sort of JPEG, TIFF or Image file that a program stores.  This data can give away important information on things like location or timestamps.  Typically this information gets scrubbed, but not in this case.

So in summation, a massive trove of private data was leaked because some pretty straightforward programming tennants were dismissed.
