---
layout: post
title:      "Sinatra Portfolio Project"
date:       2020-06-23 12:30:20 -0400
permalink:  sinatra_portfolio_project
---

My Sinatra portfolio project is designed to help people catalog their "epiphanies". The concept is based on many popular blogging websites we commonly use.

Users can signup, login, and log out of the site. There are full CRUD commands for the user once they do log in, and the site is secured with bcrypt. There are validations for every view page of the program, and so other users cannot simply go to a webpage and delete someone else's epiphanies.

This was a labor of love, and I am looking forward to having my family attempt to "break" the program. I'm also excited/scared of what kinds of epiphanies they will leave on the wall.
bcrypt is a gem that can be added into rails. Once added you can place 

> has_secure_password

into your user model.

This then allows you to create a column called

>password_digest

into your db. This allows passwords to become salted and hashed as they get passed into your program. In order to pull this out of your db, you can utilize .authenticate and then pass in :password as params to identify if this is the correct password.

