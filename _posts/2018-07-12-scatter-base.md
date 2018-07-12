---
layout: post
title: Scatter Plots
---

# Hi Readers,
Let's go through the scatter plot code base and see how we can use it for other
ideas as well.
![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/8.png)

So currently the code base looks like this I have cleanly divided the scatter
code base to 4 different files based on the applicability.  

Lets walk through the crucial steps of the development process.

```
plot = Rubyplot::Scatter.new(400)
plot.data(:data1, [1, 2, 3, 4, 5], [11, 2, 33, 4, 65])
plot.write('spec/reference_images/scatterplot_testplot_1.png')
```

**This code works internally in the library as ->**


![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/9.png)

**Which makes an image**

![webjeda hagura jekyll theme](https://raw.githubusercontent.com/Arafatk/hagura/gh-pages/images/10.png)
