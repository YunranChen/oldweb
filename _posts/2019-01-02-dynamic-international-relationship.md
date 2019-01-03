---
title: "Dynamic Network Analysis: International Relationship"
layout: post
date: 2019-01-02 14:19
tag:
- network
- statistics
- R
- time series
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


## Summary:

I am interested in modeling dynamic networks, where each edge between pairs of nodes can be seen as a time series. In this project (STA642 course project), I am trying to fit a dynamic international relationship to explore the time-varying relational structure instead of making prediction.

For social networks, the latent space model proposed by Hoff et. al. (2002, 2005) is widely used. The basic idea is to introduce a multiplicative random effect to the mix effect model. Such multiplicative random effect can induce a third dependence structure, which accommodates some typical dyadic characteristics, such as homophily and stochastic equivalence ("friends of my friends are my friends", "enemies of enemies are my friends") (Hoff 2008). However, the latent space model is for static networks. Durante and Dunson (2014) extended this model to a model for dynamic networks evolving in continuous time by setting Gaussian process for each element. Instead of considering continuous time, I consider discrete time series. Explicitly, I assume each element as a stationary AR(1) process. First, I explored the properties of product of two stationary AR(1) processes. Based on this, I derived Gibbs sampling scheme with Polya-Gamma augmentation for posterior computation. Then I did extensive simulations on the choice of parameters and applied the proposed model to analyze the real dataset. At the end I provide detailed discussion on the limitations and further directions.  



Reports and codes please refer to my github <a href="https://github.com/YunranChen/DynamicRelationship">Dynamic Relationship</a>.
