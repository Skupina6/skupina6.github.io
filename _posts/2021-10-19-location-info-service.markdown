---
title: ":world_map: Location info service"
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

Reddit is a social network allows you to upload photos. Users can view a lot of impressive photos of different locations. However, currently it is not possible to add a location metadata a certain photo.

The idea for this project came from lack of this feature. Users would benefit having a way to *mark* photo with location, so they would be able to search all content  taken within some country, city or region. Also, it would be usefulto have all relevant data regarging certain location. 

In a scope of this project I built a automated account that responds to comments where it is mentioned (text that includes unique username of the account). The mention comment acts as a search command for location. For example:

> u/LocationInfoBot Crawford path

![Location info bot response](https://user-images.githubusercontent.com/11059438/111335197-79a33700-8674-11eb-8ee7-f259ad3946a1.png)


Bot will return location description, list of nearby location, relevant links: wikipedia, map, hotels, hiking, thumblr, pinterest. This automated account helps users improve SEO of their content - users can use Reddit search engine to easier find such content or filter content by location .


##  Technical details

Application is built using Python (Django), APScheduler and PRAW.
