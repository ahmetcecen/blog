---
slideinit: "<section markdown=\"1\" data-background=\"http://matin-hub.github.io/project-pages/img/slidebackground.png\"><section markdown=\"1\">"
vertical: "</section><section markdown=\"1\">"
horizontal: "</section></section><section markdown=\"1\" data-background=\"http://matin-hub.github.io/project-pages/img/slidebackground.png\"><section markdown=\"1\">"
subtitle: ""
layout: post
author: Ahmet Cecen
tags: class materials-informatics
theme: beige
trans: cube
visualworkflow: false
published: true
title: Understanding 2-Point Statistics
category: class
date: 2016-10-04 10:30
---

# Frequentist Approach

> If I threw a particular vector at every possible location in this image, what fraction of them will land both on white pixels.

![Freq.png]({{site.baseurl}}/img/tutorial-resources/Freq.png)

# Bayesian Approach

> I have a paper with 2 holes in it seperated by a particular vector. If I put this paper on a random location on top of the image, what is the probability that I will see a white pixel on both holes, given both holes reside within the image.

![Improc.png]({{site.baseurl}}/img/tutorial-resources/Eq.PNG)

<video style="display:block; margin: 0 auto;" width="700" height="500" controls>
  <source src="{{site.baseurl}}/img/tutorial-resources/capture.webm" type="video/webm">
Your browser does not support the video tag.
</video>

# Topological Approach

> Normally, the location of each pixel in the image is described by a vector from the x axis, and a vector from the y axis. If I instead describe each white point, by vectors from every other white point in the image, how many times would I observe a particular vector (normalized by the number of points/vectors).

![Improc.png]({{site.baseurl}}/img/tutorial-resources/Improc.png)

