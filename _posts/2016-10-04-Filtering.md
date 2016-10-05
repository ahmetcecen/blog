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
title: 2-Point Statistics & Filtering
category: class
date: 2016-10-04 10:40
---

# Graphical Explanation of Filtering

Let us assume we have the following matrix, or image.

![Mat.png]({{site.baseurl}}/img/tutorial-resources/Mat.png)

We are interested using this filter on our image.

![Filt.png]({{site.baseurl}}/img/tutorial-resources/Filt.png)

A filter is applied on an image by placing it centered at every possible location on an image, multiplying the values of the filter and the current subsection of the image corresponding to the location of the filter. The multiplied values are then summed up and the resulting value is placed at the pixel the filter was centered on. 

Here is a detailed graphic of a single step.

![Filtering1.png]({{site.baseurl}}/img/tutorial-resources/Filtering1.png)

Repeat this for every pixel.

![Filtering2.png]({{site.baseurl}}/img/tutorial-resources/Filtering2.png)

How do we deal with the boundaries? Many ways, but for our purposes, we will either assume that one end of the image is connected to the other (periodic boundary) or there is nothing (zeros) beyond the boundary (non-periodic boundary).

![BoundaryFilt.png]({{site.baseurl}}/img/tutorial-resources/BoundaryFilt.png)

# Filtering for 2-Point Statistics

For efficient calculation of 2-point statistics, we use the image itself (phase of interest marked with 1s, all other phases marked with 0s) as both the input and the filter.  Graphical examples of how this would work are given below for 2 vectors.

One step.

![Ex1.png]({{site.baseurl}}/img/tutorial-resources/Ex1.png)

Another step.

![Ex2.png]({{site.baseurl}}/img/tutorial-resources/Ex2.png)

It follows that the resulting matrix will give us the counts of succesful trials in the frequentist definition of 2-point statistics, for each vector. Normalization will yield the actual frequencies.