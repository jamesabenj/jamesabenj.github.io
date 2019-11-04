---
layout: post
title:      "Some Thoughts on OO and Scraping. "
date:       2019-11-04 09:52:19 -0500
permalink:  some_thoughts_on_oo_and_scraping
---


Object Orientated Ruby definitely put me through my paces. The biggest challenge being understanding the relationship between classes and how they can interact across multiple files. The challenge as it relates to my first project, a CLI app that scrapes Steam, was in dealing with dynamic data. I decided to use the top 100 most popular games by player count, a table that can change by the hour. The key was in being extra careful in the CSS selectors that I chose. The wrong one and the app could break or display the wrong information. Of course the best tool, and one I used often was Pry. It’s super handy to be able to nail down those return values as you go. I don’t know what I would do without it.  
