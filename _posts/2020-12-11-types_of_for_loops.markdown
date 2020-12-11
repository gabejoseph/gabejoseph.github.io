---
layout: post
title:      "Types of for Loops"
date:       2020-12-11 14:56:31 +0000
permalink:  types_of_for_loops
---


This week I spent some time working through different iterators and have spent some time looking into what makes each unique.  During your time at Flatiron there is a high liklihood you'll see a section on the difference between forEach and .map for example.  This is going to wind up being important because of all of the types of interators JS offers you.  The two I will be focusing on here are 

> for (let index = 0; index < array.length; index++) {
>     const element = array[index];   
> }

And 

> for (let x of Array) {
>     console.log(x)
> }

There is a key difference here and it is a functional one.  With the array above you can indicate positions in the array you're iterating through in an effort to specifically modify elements.  The second loop just has you move through each stage in the array and is much more akin to something like .map.
