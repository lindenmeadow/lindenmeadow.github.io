---
layout: post
title:      "Reflecting on ReflectionTime"
date:       2020-03-30 17:27:00 -0400
permalink:  reflecting_on_reflectiontime
---


It's hard to believe that it's been so long since my last blog post. Granted, I had some family issues and other circumstances that caused me to stall out on my web development studies with Flatiron, but I feel relieved to be back in the game. 

Creating the CLI web scraper for my first portfolio project was satisfying -- not mention challenging -- enough. Creating the Sinatra portfolio project was even more so. After days of reviewing the Sinatra and ActiveRecord lessons, as well as watching a number of tutorials and demonstration videos on YouTube, I finally was able to hammer out what I felt was a decent CRUD app. 

Just settling on a project idea proved a challenge. For a while I considered creating an app that would allow teachers/instructors to record their students' grades, i.e., an electronic grade book. However, I spent some time talking with my wife, who teaches 3rd grade in a nearby public school, about apps that could prove useful for a teacher such as herself. I finally settled on creating a prototype of an app that would allow her students (and, presumably, students in other teachers' classes, and possibly students in other schools in the district) to submit reflections on their projects over the school year. 

Being a CRUD app, this program, which I decided to call ReflectionTime, would allow users to sign up/login, edit their login credentials (username and password),  view their reflections and reflections submitted by other users, create/edit/delete their own project reflections, and logout. The app is designed so that a user can edit and/or delete *only* his/her own reflections. 

There are two models: User and Reflection. The User model 'has many' reflections; the Reflection model 'belongs to' a user. In the database ('db'), the CreatUsers class has two columns: username (shortened to 'name') and password. The CreateReflections class has multiple columns, for properties such as the student's name, the project's name, the kind of project, and feedback on different aspects of the project. 

There are three controllers: an application controller, a user controller, and a reflection controller. Each of these has appropriate RESTful routes that enable the app to perform the functions mentioned above. 

Finally, there are ten '.erb' files in the 'views' folder. First, a layout page dictates the standard structure for each of the pages in the app. Next, there is a landing page that users will see when they first activate the app. The remaining eight files in the folder are equally divided between two subfolders: a 'users' folder and a 'reflections' folder. Following standard file naming conventions, I gave the various files names such as 'index', 'login', 'show', etc. To facilitate creating and styling these pages, I used Bootstrap, though I created a number of CSS style rules of my own. 

Probably the most challenging aspects were figuring out the necessary coding for the RESTful routes in the controllers and getting the embedded Ruby to work with the HTML. Much more debugging than I had anticipated turned out to be necessary, requiring me to burn the midnight oil sometimes to figure out why I kept getting certain error messages over and over or why the app wouldn't always do what I wanted it to. I remarked to a relative recently that I can now relate all too well to a  joke I've seen programmers share:  'The program doesn't work, but I don't know why .... The program does work, but I still don't know why.'" 

If you'd like to view my code, here is my [github repository](https://github.com/lindenmeadow/reflectiontime). 

And a shoutout to those who created all the helpful videos on YouTube and those who shared their CRUD app repositories. I couldn't have done it without them. (I can also understand now why they say that web developers spend more time researching solutions than they spend writing code!)












