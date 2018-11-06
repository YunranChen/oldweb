---
title: "Python Package: Variational Inference on Latent Dirichlet Allocation"
layout: post
date: 2018-07-09 17:45
tag: 
- statistics
- Python
image: /assets/images/markdown.jpg
headerImage: false
projects: true
star: false
description: "Dynamic network analysis on Higgs Boson twtter data."
category: project
author: yunranchen
externalLink: false
---


One of the core problems of modern statistics is to approximate hard-to-compute probability densities. This problem is especially important in Bayesian statistics for posterior density approximate under complex hierarchical structure setting (the one that includes latent variables). Variational Inference (VI) is a method that approximates probability densities through optimization. VI is faster and easier to scale to large data compared to classical methods, such as MCMC sampling. Here we implemented variantional EM algorithm on Latent Dirichlet allocation (LDA). Latent Dirichlet allocation (LDA) is a three-level hierarchical Bayesian model for collections of discrete data, such as text corpora. We present Variational EM on LDA model based on Blei \etal,2003 . We present detailed introduction and proof, detailed psudocode, and a package (VIonLDA). We also present the algorithm optimization based on vectorizaiton version which can be extended to not only one-hot-coding matrix. Then we provide an application on a real dataset and get reasonable result. In addition, we present detailed VI algorithm for smoothing LDA. At last, we provide a detailed discussion on ideal data structure.

Reports and codes please refer to my github <a href="https://github.com/YunranChen/VIonLDA">Python Package: Variational Inference on Latent Dirichlet Allocation</a>
