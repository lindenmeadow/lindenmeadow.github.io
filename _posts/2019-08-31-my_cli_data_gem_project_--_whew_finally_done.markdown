---
layout: post
title:      "My CLI Data Gem Project -- Whew! Finally Done!"
date:       2019-08-31 16:36:16 +0000
permalink:  my_cli_data_gem_project_--_whew_finally_done
---


When I first looked over the instructions for the CLI Data Gem Project, I felt quite overwhelmed. The OO labs had proven challenging enough, often requiring me to Google solutions for them. And frankly, I was still trying to figure out how all this Ruby code worked together. How the heck was I going to figure out how to create a Ruby data scraper that would meet Flatiron's requirements, as well as complete all the side items, especially creating a demonstration video to upload to YouTube -- something I had no idea how to do. 

I stalled on the project for several weeks for multiple reasons. Aside from the challenge of figuring out how to create the data gem itself, interruptions of various kinds kept arising, from my work and home responsibilities to helping my aging parents. Wanting to finish up Flatiron's course in under a year, I got exasperated with the delays. Further frustrating me was how, after I would ask for feedback from my Flatiron advisor, she would keep insisting that my work wasn't demonstrating sound OO design principles. (I mean, the thing worked, so why the heck did I need to keep tinkering with it?)  In all honesty, there were times when I wondered if enrolling in the course had been worth it. However, the point of the assignment was for us to improve our grasp of OO programming with Ruby, so I soldiered on. 

After a lot of trial and error, not to mention a lot of time watching YouTube videos about CLI data gems and studying others' CLI data gem code, I at last created a well-functioning project of my own that met my Flatiron advisor's approval.

So, just what sort of data gem did I create? 

After considering several options, I settled on a gem that would scrape news headlines from a web page, present them in a numbered list, and then allow the user to select a headline to view a short teaser about that news story and the story's URL. The user can then select another headline, view the complete list of headlines again, or exit the program. The web page I chose to scrape was catholicnewsagency.com/headlines, prompting me to name my gem CatholicNews.

Initially, I planned for the gem to have just two classes: a News class, which would scrape the page and assemble the data, and a CLI class, which would control the user interface. Even this was a nearly hurculean task for me, though I learned a good deal about Ruby classes, variables, and methods and how they 'communicate' with each other. For instance, I learned a good deal about whittling away unnecessary or unworkable code. My News class had five methods: three that scraped and collected the headlines, teasers, and URLs, respectively, and two for accessing the arrays that held the teasers and URL. My CLI included a greeting, input options, and code for listing the headlines and presenting a story's teaser and URL.

My Flatiron advisor still wan't satisfied and kept recommending that I add an additional class that would instantiate an article/story object. I was tempted several times to just submit what I had completed, but I suspected Flatiron's reviewers would send it back to me for refactoring. I had tried creating a Story class before, but for the life of me I hadn't been able to figure out how to create one that would be compatible with the News and CLI classes that I had developed. Well, back to the old drawing board...

Probably one of the most important lessons I've learned so far from Flatiron's program is that it is often imperative to seek assistance when completing a project. In fact, when I have brought this matter up with other Flatiron students, they remarked that was probably one of the aims of our lessons -- to teach us to search for solutions and/or ask for help from others. I've read that even professional programmers and web developers frequently have to do that, as there is just too much for anyone to learn and figure out on their own. 

I kept experimenting and researching, all of which finally paid off. Yes, I had to rework much of my code, but I succeeded in creating a gem with structure that "looks super clean" (in my advisor's words) and does a better job of following OO design than my initial efforts had. My gem includes a Story class that instantiates story objects, a News class for scraping the page, and a CLI class for the interace. I also included the colorize gem to add some color to the displayed output. 

The only thing left for me is the demo video, which I will create with OBS Studio -- another thing I've had to learn how to use. I'm looking forward to moving on with the course. SQL, anyone?
