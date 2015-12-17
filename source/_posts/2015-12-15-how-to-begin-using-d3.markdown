---
layout: post
title: "5-Minute Guide: how to begin using D3.js"
date: 2015-12-16 22:55
comments: true
sharing: true
footer: true
---

![D3 visualization from ](http://i.stack.imgur.com/JPYn9.gif)
source: http://stackoverflow.com/questions/18056678/hiding-text-elements-in-d3-chord-diagram

### What is D3.js?
###### R2D-who? More like D3, *honey.*

You've probably heard about D3 or seen D3 in action before - if you've ever seen any awesome information graphic in the New York Times in recent years... probably D3. Maybe you arrived here because you need to make an infographic, maybe you.  In any case you're embarking on an important next step in information storytelling.

If you're reading this, it's basically a fact that you've had to make some sort of chart, graph, or information visual in your life.  Perhaps you used Excel or Powerpoint or Adobe Creative or even CSS (ok, I see you!). No matter your method, if you've ever gone about sharing it, you have probably encountered the common dilemma that data today changes.  Fast.  By the time you've made your static visual and posted it on your blog, it's already out of date.

Enter [D3.js](http://d3js.org/) - a Javascript library\* that provides methods for rendering dynamic data visualization in browser through an intricate dance of HTML, CSS, and the data you want to visualize.

\*(a Javascript library, in case that's an unfamiliar term, is essentially a set of extra methods that have been pre-made for you out of existing Javascript functionality.)

> ##### The first time I heard of D3, it was like, <br>"oh wow. oh wow. oh. wow."

>It was exciting. It was tactile. It was beautiful sexy.

Disclaimer: you're going to be much better off attempting this if you're comfortable with HTML, CSS, Vanilla (basic) Javascript, and at at least some understanding of DOM manipulation.
### 5 steps in 5 minutes to get started: ###
- Step 1 - [Go here](https://github.com/mbostock/d3/wiki/Gallery) and copy the HTML and JSON of the file you like and save them each as their own files in the same local directory.  See my list of easy-to-use favs below.
- Step 2 - Set up your local host - find the command you need [through this link](https://github.com/mbostock/d3/wiki#using), then run that command in terminal when you're in the same local directory
- Step 3 - in Chrome, navigate to the local host you've opened. This will likely look something like `localhost:8888` in your search bar.
- Step 4 - Tinker: see below.
- Step 5 - Enjoy.

#### Fav beginner-level examples from the D3 site:

- [A cool force-directed Les Miserables character map](http://bl.ocks.org/mbostock/4062045)
- [A tree showing nested-layered info](http://bl.ocks.org/mbostock/4063550)
- [A fun particle thing](http://bl.ocks.org/mbostock/280d83080497c8c13152)

#### How to Tinker with the sample D3's from their site.

Once you've got your example HTML file and JSON file in front of you, you're ready to see if you can prod this thing to make it jump. But to do that, you actually need to know a bit of D3 syntax.  Anywhere in your JS or HTML, when you see "D3.[method]", that's essentially "Document.[method]", having D3 methods called on it. Here's a shortlist for deciphering what you're reading:

`selection.data` - This is the big boy. This is called the "data join" and it is the heart of how you incorporate your data set into the DOM. See more on data join basics [halfway down this page](http://bost.ocks.org/mike/bar/).

`selection.attr(something)` - setting an attribute

`selection.style(something)` - declaring the CSS-styling of the selection.

`selection.property(something)` - imbuing the selection with a property (all these are well-named, no?)

- the 3 previous methods allow you to hard-code the "something" inside, but also to pass in a function that will dynamically generate that something depending on each data point. Syntax like so: `selection.text(function(d) { return d; });`


`.domain(value1,value2)` - this is where you declare the domain of your data.

`.range(value1, value2)` - and this is where you declare the range of pixels to which you want it to map.


#### Enjoy.
D3 allows us to create visualizations that are dynamic, that can easily change, that can update as often as the data that they visualize might.  It's a bit of a learning curve at the start (I'm still on the curve), but so so pretty wow and worth it.

---

###### Further Resources:


- [This guy](http://www.jeromecukier.net/blog/2015/05/19/you-may-not-need-d3/) is great. He blogs about D3 often.
- [Here's a great game to waste a lot of time](http://color.method.ac/) , built with D3. Thanks, D3.
- Basically, [all things mbostock](http://bl.ocks.org/mbostock).
