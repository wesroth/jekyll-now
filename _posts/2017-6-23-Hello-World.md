---
layout: post
title: Genetic Algorithms and Alloys - Introduction and Overview.
---

## Introduction

  Materials Optimization, especially when it comes down to linking microstructural features to desired properties, boils down to an effective search optimization problem. Subsequently, exploring various algorithms that can efficiently compute desirable properties from phenomological linkages such as grain boundary strengthening, precipitation dispersion, solid solution strengthening, and ductility measurements will lead to ideas on the type of processes necessary for production of optimized compositions and microstructures.

  This is not novel, and this post, in part is merely a recreation and hopefully eventual expansion of the subsequent paper by [Kulkarni et. al.](http://www.sciencedirect.com/science/article/pii/S0921509303014722) in 2004, before it was hip. Furthermore developments using Artificial Neural Network methods have been published and are worth reading as [well](http://www.sciencedirect.com/science/article/pii/S0921509316301678), however as both an exercise to myself and general usefulness to retain what coding skills one has, I am doing a comparative walk through of designing a genetic algorithm for microstructural optimization of a single phase Aluminum alloy variant. For more complicated microstructures, such as that featured in alpha-beta Titanium alloys (looking at you Ti-6-4), you can also derive phenomological models but be prepared for dealing with a flustering amount of variables, see above link.

  Overall, this is essentially going to be an application of a more faceted, material-science based genetic algorithm than what can be found in this excellent tutorial, linked [here](https://lethain.com/genetic-algorithms-cool-name-damn-simple/).

  This will probably be a multi-part posting just due to the immensity of material (no pun intended) and background. Thus a general table of contents would follow:

   1. Introduction.
   2. Material Science Fundamentals and Ramblings
   3. Genetic Algorithm Breakdown
   4. Putting it all together - Coding Time
   5. Where to go from here...


   *Disclaimer: Since Python is the preferred language for myself and for all intents and purposes is fast enough to handle what we are dealing with, as well as accessible with it's respective scientific computing libraries, it will be conducted here. That being said, I am no Python expert, nor will this code be well optimized or Pythonic like the snippets by the girls and boys on Stack Overflow.*


## Goal

**The overarching goal is thus to optimize a microstructure based on considerations of yield strength, high temperature strength, and ductility.**

Using phenomological equations for these material properties, a genetic algorithm will search for the optimal microstructural features for a given target.

Next time, we begin with the fundamental material science behind why we care about this all in the first place. 
