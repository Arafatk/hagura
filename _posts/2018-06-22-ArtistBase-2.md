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
