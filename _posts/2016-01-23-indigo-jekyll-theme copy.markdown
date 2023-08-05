---
title: ":telephone: Apartment phone number scraper"
layout: post
date: 2020-01-10 22:10
tag: 
 - django
 - python
 - scraper
# image: https://sergiokopplin.github.io/indigo/assets/images/jekyll-logo-light-solid.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: "Reads phone numbers from listings and adds them to Google contacts and links them to online content"
category: project
author: matej
externalLink: false
---

The idea for this project came from the (long) process of looking for an apartment. Currently, there are multiple platforms for real-estate listings, but every one has its problems.

First problems is that the listings dont always include all of the details. In this case, user would need to call the contact mentioned in the listing to get all the information. With a large number of contacts, it becomes hard to keep track of all relations between contact and listings. 

Initial project enabled listing notifications trough Discord. This allowed it to send metadata, links, images and phone numbers. Later version of the app added functionality to automatically add phone numbers (associated with listing) to users phone contacts (Google People app)

This application does not have user interface, instead it is a scheduled application. User defines url where the app will get data for real-estate listings and selectors for real-estate title, description, and phone number. When run, application will scrape those parameters and add them in Google Contacts.

While this application was originally meant for real-estates, it can also be used for other web apps, like car or phone selling websites. User only needs to change data selectors.


*Techincal details*

Application is built using Python (Django), APScheduler and Google Python libary.
