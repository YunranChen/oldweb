---
title: "Tutorial for Network Analysis Using R"
layout: post
date: 2019-03-22 14:31
tag:
- network
- statistics
- R
- tutorials
image: /assets/images/markdown.jpg
headerImage: false
projects: true
hidden: false # don't count this post in blog pagination
star: false
description: "Dynamic international relationship modeling for STA642 time series project"
category: project
author: yunranchen
externalLink: false
---


I serve as a <b>teaching assistant</b> for <a href="http://www2.stat.duke.edu/courses/Spring19/sta650.001/">STAT650 (Spring 2019)</a>. I prepare a <b>detailed tutorial</b> for my lab, which covering the <b>basic network analysis using R</b>. 


### Outline 

<ul>
    <li>Basic introduction on network objects. </li>
    <ul>
        <li>R packages including `igraph`, `statnet` (including `sna`, `network`).</li>
    </ul>
    <li>Collect network data:</li>
    <ul>
        <li>API requests using R packages (`rtweet`, `Rfacebook`, `RedditExtractoR`, `imdbapi`, `omdbapi`).</li>
        <li>API requests from R directly (`rjson`, `jsonlite`)</li>
        <li>Useful websites: <a href=https://github.com/briatte/awesome-network-analysis>Awesome Network Analysis</a></li>
    </ul>
    <li>Fancy visualization (static and dynamic networks):</li>
    <ul>
        <li>`ggplot2` version: `ggnet2`,`geomnet`,`ggnetwork`</li>
        <li>Interactive network visualization: `ggplot2` + `plotly`, `visNetwork`</li>
        <li>Dynamic network visualization: `ggnetwork`, `ggplot2` + `gganimate`, `ndtv`</li>
    </ul>
    <li>Network analysis using package `amen`, `statnet`.</li>
</ul>
    

Please refer to my github <a href="https://github.com/YunranChen/STA650Lab">STA650Lab</a> for more details.
