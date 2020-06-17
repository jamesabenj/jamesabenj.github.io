---
layout: post
title:      "Handling Challenges in Building 'Fetch' "
date:       2020-06-17 17:40:45 +0000
permalink:  handling_challenges_in_building_fetch
---


For my third portfolio project for Flatiron School, my domain drew inspiration from my current situation(being in the proccess of finding a dog to adopt). My "Fetch" app allows users to browse and post adoptable dogs. While building this out I ran into a couple challenges and some questions needed to be answered:

1. A dog would obviously need an image attribute so: "How to tackle image upload?"

This was probably the most time consuming part of building this app. I did alot of research and tinkering with different strategies. I ultimately decided to use the 'carrierwave' gem with Amazon's service: S3, for storage. It wasn't the easiest getting everything set up, but once everything was configured properly I found this setup to be really cool. The way you fetch images requires very little return value manipulation, which I've found to be one of the most challenging parts of web development so far. 

2. "How to set up a sensible many-to-many relationship?"

To meet this I decided to make a favorites system where a user can favorite a dog, resulting in that dog being easily viewable through a "Favorites" tab. A dog can have many followers through favorites and vice versa. This setup is also cool because it would then be easy to implement a view for the most popular dogs on the site.

