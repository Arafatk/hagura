---
layout: post
title: Thoughts on Bubble Plots...
---

# Hi Readers,  
I have had a lot of fun making cool plots and designing their geometry from
scratch because it offers a lot of interesting ideas both to understand
OOP and geometry/math.   

In this blog, I would share you the whole thought process so that you too can
make plots like that.

Let's start with the textbook definition of bubble plot
*A bubble chart is a type of chart that displays three dimensions of data. Each
entity with its triplet (v1, v2, v3) of associated data is plotted as a disk that
expresses two of the vi values through the disk's xy location and the third
through its size.*    

Practically, we can think of Bubble plot as a visualization that helps compare
the intensity of datapoints in a 2d space. For example let's look at a very classic
bubble plot     

![](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/11.png)
Here we have a 2-d space that shows a map of the united states and the diameter of
different circles helps us compare the population in different states.
This idea can also be mapped to many other plotting tasks

Now that we know **why** we make bubble plots lets move to the **"how"**.

The whole bubble class code base is divided into 3 files      
![](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/12.png)

**init.rb** -> Initialization the bubble class      
**draw.rb** -> Compilation of drawing functions     
**data.rb** -> Operations to get geometry information from the user data      

Overall, I have made a simple bubble class that inherits from scatter plot because
scatter plot and bubble plot are very similar at their core ideas. To get into the
inner runnings lets run some code and explore how it works.  


```
plot = Rubyplot::Bubble.new
plot.data(:apples, [-1, 19, -4, -23], [-35, 21, 23, -4], [45, 10, 21, 9])
plot.data(:peaches, [20, 30, -6, -3], [-1, 5, -27, -3], [13, 10, 20, 10])
plot.set_colors_array(%w[white yellow])
plot.write('spec/reference_images/bubble.png')
```

**This code is implemented internally in the library as ->**


![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/14.png)
