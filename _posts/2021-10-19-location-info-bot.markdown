---
title: ":world_map: Location info bot"
layout: post
date: 2021-10-19 05:10
tag: 
 - reddit
 - python
 - scraper
#image: https://user-images.githubusercontent.com/11059438/111335197-79a33700-8674-11eb-8ee7-f259ad3946a1.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: "Gets more details about location where photo was taken"
category: project
author: matej
externalLink: false
---

Reddit is a social network allows you to upload photos. You can view a lot of impressive photos of different locations, however it is not possible to "tag" a certain photo with a location.

The idea for this project came from this. I was looking for a way to *mark* photo with location, so I would be able to search all photos taken within some country, city or region. Also, I was looking for a way to quickly provide relevant information regarging certain information. 

In a scope of this project I built Reddit bot (automated account) that responds to its mentions (text that includes unique username of the bot). The mention comment acts as a search command for location. For example:

> u/LocationInfoBot Crawford path

![Location info bot response](https://user-images.githubusercontent.com/11059438/111335197-79a33700-8674-11eb-8ee7-f259ad3946a1.png)


Bot will return location description (which can later be searched), list of nearby location, relevant links: wikipedia, map, hotels, hiking, thumblr, pinterest. Facebook and instagram links were removed in order to avoid post removals.

Other advantage of using this bot:
- faster than googling for relevant links
- on phone you dont need to switch between Reddit and browser app
- you can search for posts by location keywords (country, region, nearby locations etc.)


**Techincal details**

Application is built using Python (Django), APScheduler and PRAW.
