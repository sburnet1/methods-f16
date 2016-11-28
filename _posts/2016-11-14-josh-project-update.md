---
layout: post
title: 'Project Status Update for Nov 14'
author: Josh
---

For a few days this week I wasn't sure if I could bring myself to finish this project and I considered starting over with a new research question. I kept thinking to myself that the events of early Wednesday morning provided all the evidence needed to show that tweeting about debates is pretty useless. I didn't really feel up to reading through the tweets supporting the actions and rhetoric of a xenophobic, sexist, grabby, racist Cheeto, as I fear that the hopes expressed in these tweets paint a picture of what will become of America... Without going into details, a lot has happened over the past few days. After witnessing the reality of our post-election 2016 America first-hand, I've decided that it's important to future elections to continue this project, on the off chance that I find something novel (and also important). (Also, as you may notice, the update/plan that follows doesn't actually require that I read any of the tweets, which will probably spare me a lot of aggravation.)

Since my last update, I've started writing a Python script to get the Tweet IDs for each tweet and use that to query the Twitter API to get the hashtags for each tweet. So far, I've managed to convert the CSV file to JSON (not strictly necessary, but I've had pretty bad luck working with CSV files in Python but working with JSON data is more familiar to me). The next step is to write a function to make the actual GET requests. I'm pretty confident I'll have this figured out within the next couple of days. After grabbing the hashtags for each tweet, I'm going to dump most of the data, reorganizing it by user. I want to have a list of users in the dataset, and then a list of hashtags used by each user. From there, I'll use the Twitter API again to get a list of who each user follows / who follows each user, and append that to the data for the users.  That should end the data-collection process.

Once I'm done making GET requests, I'll probably have to put the data back into a CSV, or some other format that will work well with Gephi. I've been reading up on Gephi, and I'm pretty sure that, once I get the data into the program, doing what I want to do should (I hope) be pretty straightforward. The goal is to end up with a few different visuals.  I'm debating whether it makes sense to use users as nodes and trying to show the distance between users *and* the distance between the hashtags they use, or whether it would be more straightforward to just use hashtags as nodes and show the distance between hashtags. I'll probably play it by ear.

From there, it'll just be a matter of making things look pretty and writing up an accompanying report/article that shows how whatever it is I find fits into (or doesn't fit into) the bigger picture of existing literature on Twitter use and social-networks/networking.

[My code is here on GitHub](https://github.com/jbguberman/dh_final_project). I'm pretty sure that everything that has to happen *after* I finish writing my code will go quickly. I might update this again before class on Monday if I make significant progress between now and then (it's Saturday night as I write this), but I plan on spending most of that time fighting fascism. ☭