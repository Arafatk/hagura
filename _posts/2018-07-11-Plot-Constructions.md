---
layout: post
title: Plot Constructions and Divisionism
---

# Hi Readers, 
I want to introduce you to the ideas behind the construction of a plot
 on top of Artist layer itself.  

But before we talk about the code let's take a step back and talk
about paintings and art in general.  
As an art aficionado, I have always loved different styles of art
and while I can't comprehend the intellect and the effort that goes behind making
beautiful paintings I love a few styles in particular like *Divisionism*.


![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/4.jpeg)

*Divisionism*, in painting, the practice of separating color into individual dots
or strokes of pigment. It formed the technical basis for *Neo-Impressionism*.

Think of Rubyplot as a programming equivalent of Divisionism where we take a
whole mathematical plot and divide it into small segments. Take for example
this simple scatter plot.   

![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/4.jpeg)

You can simply dissect it in a simple fashion by identifying all the different
drawing elements in this image which are
* Axis
* Axis Labels(The numbers 30, 40, 50 written on the left of y axis.)
* Legends(The different data sets 1952, 2017.)
* Line Markers(The horizontal and vertical light shaded lines on the graph that
  help read the data properly by identifying the closest y axis mark.)
* The circle data points placed all over the plot.

The whole idea behind our library is to make sure that we can take a look
at any plot and dissect it's geometry and then automate the construction
from on any dataset by normalizing(scaling) the data to fit within the plot
geometry. In the next post we will analyze the scatter plot in more detail.
