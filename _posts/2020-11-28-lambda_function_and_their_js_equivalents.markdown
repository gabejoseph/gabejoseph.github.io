---
layout: post
title:      "Lambda Function and their JS Equivalents"
date:       2020-11-28 17:19:06 +0000
permalink:  lambda_function_and_their_js_equivalents
---


This week I've been wrapped up in transcribing python functions into their JS equivalents.  For this post though, I'll be focusing primarily on the Lambda function and what its actual use is in python and how it translates into JS.

Take for example:

> n = lambda a: a / 5
> print n

This would be a simple function that takes in a variable a, and divides it by 5.  After this we call the variable which the function has been set to and we return a result.  Simple enough.

Lambda functions can also take in any number of variables, so we could presumably have something like:

> n = lambda a, b, c: a + b + c 
> print n

Where now we are getting the summation of a, b and c.


