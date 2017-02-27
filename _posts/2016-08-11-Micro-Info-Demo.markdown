---
layout:     post
title:         Microstructure Quantification Through Spatial Statistics
author:     Ahmet Cecen
tags: 		post R Shiny
subtitle:  	An interactive presentation of spatial statistics and PCA
category:  class
---
<!-- Start Writing Below in Markdown -->

<style>

iframe.shiny{

margin-left: -12.5%;    
width: 125%;
overflow: hidden;
position: relative;
height: 1580px;

}

@media only screen and (max-width: 930px) {

iframe.shiny{
 
margin-left: 0%;    
width: 100%;
overflow: hidden;
position: relative;
height: 2971px;

}

img{
width:100%!important
}

}

</style>


<!--
<iframe src="http://127.0.0.1:4117/" frameborder="no" class="shiny" height="1000px"  ></iframe>
-->


# 2-Point Statistics

- 2-Point Statistics can capture inherent structural organization in data irrespective of positioning, frame, window size or origin.

<img src="/blog/img/ideas-post-images/StatsExample.PNG" style="width:70%">

- 2-Point Statistics can highlight inherent lenght scales in the structure.

<img src="/blog/img/ideas-post-images/2ptExample.PNG" style="width:70%">

More about [2-Point Statistics](http://immijournal.springeropen.com/articles/10.1186/s40192-015-0044-x).

# Principal Component Analysis

<img src="/blog/img/ideas-post-images/PCAExp.PNG" style="width:100%">

PCA is a dimensionality reduction technique that extracts orthogonal features that reflect the greatest variance in data.

More about [PCA](https://en.wikipedia.org/wiki/Principal_component_analysis).

# Interactive Exploration

## Example Random Dataset

<img src="/blog/img/ideas-post-images/Classes.png" style="width:80%">

## Exploring the Microstructure Space

In case of user overload, you can also access the following app at:

- [ShinyApps.io ](https://ahmetcecen.shinyapps.io/MatInfDemo/)
- [Digital Ocean](http://198.199.121.158:3838/MatInfDemo/)
- [My Home Computer](http://73.43.183.88:1412/)

You can also find some quick picked example patterns [here](https://ahmetcecen.github.io/blog/class/2016/08/26/example-patterns/)

<iframe src="https://ahmetcecen.shinyapps.io/MatInfDemo/" frameborder="no" class="shiny"  ></iframe>

# Function Estimation

We can use the above representation to fit functions of the form:

 **Property = f(PC1,PC2,...)**.

<img src="/blog/img/ideas-post-images/Fit2.png" style="width:100%">

# Reconstructions 

We can then explore the reverse problem of how the structure would look like given a desired property value.

<img src="/blog/img/ideas-post-images/Reconstruct.png">







