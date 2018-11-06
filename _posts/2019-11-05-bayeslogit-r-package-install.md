---
title: "BayesLogit: Instruction for installing R package BayesLogit"
layout: post
date: 2018-11-05 16:18
tag: 
- statistics
- R

image: /assets/images/markdown.jpg
headerImage: false
star: false
description: "An instruction for installing R package BayesLogit."
category: blog
author: yunranchen
externalLink: false
---

To sample from PolyaGamma distribution, we could use the `rpg` function in R pacakge `BayesLogit`, which applys effecient algorithm and is written in C.

Since `BayesLogit` is removed from CRAN, here follows an instruction to install R package `BayesLogit` from github. Notice the `rpg` function may not work when the shape parameter is greater than 170, since the normal approximation may not make sure the samples are greater than 0.

1.Make sure you have installed gcc (Compiler for C).

  - For MacOS, go to App Store, download Xcode.

  - Or use the commandline in terminal:
{% highlight raw %}
$ brew install gcc
{% endhighlight %}

2.Make sure you have right path for `gfortran`.

{% highlight raw %}
$ curl -O http://r.research.att.com/libs/gfortran-4.8.2-darwin13.tar.bz2
$ sudo tar fvxz gfortran-4.8.2-darwin13.tar.bz2 -C /
{% endhighlight %}

3.Follow the instructions in <a href="https://github.com/jwindle/BayesLogit/blob/master/INSTALL">github</a> to generate R package.

1) Get the BayesLogit code.
 
  - You can clone the repository or download the code as a zip file via
    github.com.

  - For these instructions, ASSUME the repository directory is called
    BayesLogit.

2) Install the Matrix and RNG files in BayesLogit/Code/C/include/

  - From the command line

    {% highlight raw %}
      cd to BayesLogit/Code/C/include	
      $ wget https://github.com/jwindle/Matrix/archive/master.zip
      $ wget https://github.com/jwindle/RNG/archive/master.zip
    {% endhighlight %}
  - Or from your browser
    - type in the above links and save them in
      BayesLogit/Code/C/include/

  - Unzip the files.

  - Remove the -master suffix
    {% highlight raw %}
    $ mv Matrix-master Matrix
    $ mv RNG-master RNG
    {% endhighlight %}

3) cd to BayesLogit/Code/BLPackage

4) Update the files for the package.

    {% highlight raw %}
    $ bash sync.bash
    {% endhighlight %}

5) Build the package

    {% highlight raw %}
    $ R CMD build BayesLogit
    {% endhighlight %}
6) Check the package (optional)

    {% highlight raw %}
    $ R CMD check BayesLogit_WHATEVER.tar.gz 
    {% endhighlight %}

7) Install the package

    {% highlight raw %}
    $ R CMD INSTALL BayesLogit_WHATEVER.tar.gz
    {% endhighlight %}