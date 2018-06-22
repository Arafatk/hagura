---
layout: post
title: Developing the Artist base class part-2
---

Currently the directory structure looks like this    

![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/3.png)

So we have a base folder directory where I have defined the artist class and the
goal with this is to design a super structured artist layer with a base class
that forms the basic back bone of the repo and the rest of the classes inherit
all the basic design features from this class.

What exactly are the basic design features that I speak of?  
* draw_legend
* draw_line_markers
* draw_title
* draw_axis_labels

This helps draw the basic outline for a graph thereby giving you a bare bones
plot with no data and just labels, axis, titles. On top of this we can build
anything we want. So basically the idea is to automate the construction
of a base graph as a plot with these basic functions.   

![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/1.png)     
Once, I was done with the core functions I started to build graphs on top of
it and currently I built the following types.
* Bar
* Scatter
* Dot
* Line

All these graphs have individual draw+math functions that build the whole
plot and automate the whole process as cleanly as possible.     

Let's look at a [dot graph code](https://github.com/Arafatk/magick-rubyplot/blob/master/lib/rubyplot/artist/dot/dot.rb)
 for example.   
We have a draw function it initially calls super method inorder to set up
the graph, and normalizes the data to make it easily plottable.
Then it sets the spacing for the data labels, horizontal/vertical lines and everything.
Then we calculate the positions in pixels(X+Y coordinate) for the dots and actually plot the
dot graph using circle method to make small dots on the graph.   
In a similar fashion I made other graphs too. I will focus on the complete thought process
behind building a single line graph in the next blog.
Stay tuned folks!!!
