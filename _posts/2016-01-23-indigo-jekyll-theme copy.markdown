---
title: ":ramen: Apartment phone number scraper"
layout: post
date: 2016-01-23 22:10
tag: jekyll
image: https://sergiokopplin.github.io/indigo/assets/images/jekyll-logo-light-solid.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: "Reads phone numbers from ads, adds them to Google contacts and links them to ad."
category: project
author: johndoe
externalLink: false
---

When I was looking for an apartment, I found a lot of appropriate housings. The problem was that ads for those housings did not have all the details, so I had to call owners.

The problem is that it becomes confusing when you have a large number of contacts. You dont know which number belongs to which housing owener.


So I was thinking about this problem, and I said: Wouldnt be cool if I alreads had those contacts linked with ads? So the idea for this app was born.

This application does not have UI, it is a scheduled application. Developer defines url where the scraping wil commence, and selectors for apartment title, description, and phone number. When run, application will scrape those parameters and add them in Google Contacts.

This application was initially meant for [nepremicnine.net](https://www.nepremicnine.net/). However, the best thing is that this scraper can also be used for other things, like scraping car or phone advertisements (on a webpages like auto.net or bolha.com). You only need to change data selectors.


**Techincal details**

Application is built using Python (Django), APScheduler and Google Python libary.
