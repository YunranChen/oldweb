---
title: "Causal Inference with Interference"
layout: post
date: 2019-01-02 15:22
tag:
- network
- statistics
- R
- causal inference
image: /assets/images/markdown.jpg
headerImage: false
projects: true
hidden: false # don't count this post in blog pagination
star: false
description: "Review and reproduction of the paper by Forastiere et.al., including a introduction of the extended framework and simulations."
category: project
author: yunranchen
externalLink: false
---


## Summary:


This is a course project for STA 640 Causal Inference. 

In observation studies, our target population may have a network structure. Interference may occur if the potential outcome of one unit depends on both individual treatment and neighborhood treatment. The present of interference will break down the traditional assumptions and framework. In this project, we review the paper by Forastiere \etal (2016), which provides a extended framework and solution for the existence of interference. The basic idea for the framework and assumption extension is to take neighbors into consideration, which means to extend potential outcomes, assignment mechanism and average does-response function as a function of both individual and neighborhood treatment. Accordingly, propensity score is generalized to a joint propensity score then decomposed to individual and neighborhood propensity score, from which a estimating procedure is proposed. Here we focus only on causal inference on main effect (individual effect) when interference presents. We reproduced the simulations by Forastiere et. al. (2016) based on Facebook data obtained from Stanford Network Analysis Project (SNAP)(Leskovec and Mcaule, 2012 ).


Reports and codes please refer to my github <a href="https://github.com/YunranChen/Interference_in_CI">Causal Inference with Interference</a>.
