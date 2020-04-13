---
layout: post
title:      "Quick and Dirty Graphs for Ruby Apps"
date:       2020-04-13 15:02:23 +0000
permalink:  quick_and_dirty_graphs_for_ruby_apps
---


Google Charts is a graphing api that can produce some nice charts. The problem with it is that it requires alot of javascript to get up and running, and it doesnt play too nicely if you're working with dynamic data in Ruby.  Luckily for me and my Sinatra Portfolio Project, I found the googlecharts gem. googlecharts is a wrapper for Google Charts which handles the javascript and makes visualizing data in a Ruby app a quick and easy affair. 

Now googlecharts has its issues too, primarily for the fact it hasn't received much support recently. Also, because the gem produces an image url, you lose some potential interactivity.  There certainly are better options for more complex implementation of graphs/charts for Ruby. Some of those include the likes of D3 and Highcharts. However, for quick and dirty graphs, this worked for me. 

Getting started with googlecharts is a familiar procces. First start by istalling the gem:

```
gem install googlecharts
```

then requiring it in your gemfile:

```
gem 'googlecharts'
```

Lastly, run 'bundle', and there you have it! 

Google Charts supports lots of different types of graphs, from line to pie and pretty much everything in between. You can see the gem documentation [here](https://www.rubydoc.info/gems/gchart/1.0.0) and source code [here](https://github.com/mattetti/googlecharts), as well as the official Google Charts doc [here](https://developers.google.com/chart).






