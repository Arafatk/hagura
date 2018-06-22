---
layout: post
title: Developing the Artist base class part-1
---

# Hi Readers, 
Now, that I have finally started working on my codebase let's start focussing on
most interesting problems in development and replication of Matplotlib.  
I have already written a ton about the design in [roadmap for the project](https://docs.google.com/document/d/1t7jJKMaPjFI7pbjfMSG7eh6YmqqIE0qEoXXqsxROlYs/edit)
so now I will focus more on the implementation aspect of things.

But before we start, I want to take you through a thought process. Imagine for a moment
that you have to draw a beautiful painting.

![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/4.jpeg)

*What do you need to draw a painting?*
* Paint brush and Paint  
* A blank Paper
* A design or a mental model of what you are going to draw.

The library works in similar thought process too you give it an empty paper
called figure canvas and then you draw upon the figure canvas using plotting
features. For all drawing and plotting purposes in this library we use RMagick.
![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/5.gif)

So where are our paint brushes and paints?
* draw->rectangle
* draw->circle
* draw->line
* draw->annotate

Now if you really give this some thought and think of building a plots drawn by
your own hands it's very easy to realize that every plot can actually be broken
down as a combination of the above objects. It's almost as if plotting is a
language and these are the alphabets which are put together to make a word(plot).

These are raw core features that act as the paint brush and paint for our library.
Using these together along with proper mathematical formulation for spacing,
edges, axis, lines etc helps us make beautiful plots for our library.

How we actually go about doing that is the subject of the next blog post
so please do check it out....
