---
layout: post
title: Scatter Plots
---

# Hi Readers,
Let's go through the scatter plot code base and see how we can use it for other
ideas as well.       
So currently the code base looks like this I have cleanly divided the scatter
code base to 4 different files based on the applicability.  All the files do exactly
what their names suggest.
![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/8.png)

Now let's take a look at some example code to make scatter plot.

```
plot = Rubyplot::Scatter.new(400)
plot.data(:data1, [1, 2, 3, 4, 5], [11, 2, 33, 4, 65])
plot.write('spec/reference_images/scatterplot_testplot_1.png')
```

**This code is implemented internally in the library as ->**


![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/9.png)

**Which makes an image as**

![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/10.png)

I hope this explains the whole concept of the construction of scatter plots.
