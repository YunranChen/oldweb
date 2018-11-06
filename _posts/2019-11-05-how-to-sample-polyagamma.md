---
title: "BayesLogit: How to sample from Polyagamma distributiona and some issue on R package"
layout: post
date: 2018-11-05 16:18
tag: 
- statistics
- R

image: /assets/images/markdown.jpg
headerImage: false
star: false
description: "An brief instruction for how the rpg function works in R package BayesLogit and related issues when using the function."
category: blog
author: yunranchen
externalLink: false
---

To sample from PolyaGamma distribution, we could use the `rpg` function in R pacakge `BayesLogit`, which is hybrid sampling approach based on Devroye, alternative and saddlepoint sampling method proposed by Polson et. al. (<a href="https://arxiv.org/pdf/1205.0310.pdf">2013a</a>, <a href="https://www2.stat.duke.edu/~jbw44/Papers/NewPGSamplerWriteUp.pdf">2013b</a>). Here I would provide a brief introduction on how it works.

$asd=\frac{1}{2}$