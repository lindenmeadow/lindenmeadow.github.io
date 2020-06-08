---
layout: post
title:      "Tarheel Teachers"
date:       2020-06-08 21:57:29 +0000
permalink:  tarheel_teachers
---

After viewing what seems like a thousand and one error messages, not to mention redoing my code at least twice that many times, my Rails CRUD project is finally complete. Well, it hasn't been officially reviewed and given a pass yet, but at least it does everything I want it to do. Thank heaven for YouTube tutorials, Stack Overflow, and Github. Crossing my fingers... 

For my third web development project, I've created what is intended as a message board app for educators (or people who work in the education sector) in North Carolina. (For those who may not know, North Carolina is called the Tarheel State, and its residents bear the nickname Tarheels.) However, the app can easily be adapted for use by people in any area to fit their needs/interests. 

Users must sign up and create a short profile, including a username, email address (which is kept secret), short bio about themselves, and a favorite quote about education. The controllers and models are designed so that usernames and email addresses must be unique (i.e., a new user cannot create an account with a username or email that is already being used by another account). All users can create posts (called 'discussions') and leave comments on other users' discussions. Each discussion will fall under a particular 'forum' (a broad category or topic). However, ordinary users can edit and delete only their own posts. 

As a way to add 'roles' to certain user accounts, I have included the CanCanCan and Rolify gems, which enable particular users to be designated as a 'moderator' or an 'admin'. Moderators can edit and delete other users' discussions and comments. An admin has the authority to do that as well as create and edit new forums and even delete other users' accounts. Of course, adding these roles is a way to maintain propriety and order on the app, such as by removing inappropriate or offensive discussions/comments or kicking a disruptive user off the site. Deleting an entire forum also deletes any discussions and comments in that forum (as they are dependents, as specified in the models), and deleting a user account likewise deletes that user's discussions and comments.

Now to move on to project 4...


