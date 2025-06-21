---
title: Seed Dispersal
summary: Estimate seed dispersal and seedling survival vs. distance from the parent tree.
tags:
  - Ecology
date: ''
---

Understanding how a diversity of species can coexist on the long term at a given place remains an active area of research in ecology. One popular explanation for the high local biodiversity of tropical forests is the Janzen-Connell hypothesis, according to which mature trees attract specialized predators feeding on their seeds, suppressing the emergence of seedlings close to their parent and leaving space for other species. Mathematically, this implies that whereas the *seed dispersal kernel* (the distribution of seeds vs. distance from the parent) peaks at the parent tree's location, the *effective dispersal kernel* (the distribution of surviving seedlings) peaks away from the parent.

Typical surveys aimed at measuring dispersal will map trees of the target species in a forest, then sample and identify seeds (or seedlings) in a series of small plots distributed across the forest. Because the observed spatial distribution of seeds (or seedlings) adds up the contribution of all possible parent trees, that distribution is a convolution of the dispersal kernel with the spatial distribution of mature trees, and researchers are faced with the inverse problem of estimating the parameters of the unkown dispersal kernel from the output of that convolution. Because the observed seed (or seedling) counts are a complicated nonlinear function of those parameters, they cannot be estimated via standard (e.g. generalized linear regression) methods. Bayesian networks, in contrast, can express arbitrarily complex relationships between parameters and observed data, and the parameters can be fit using Monte Carlo algorithms.

In this project, I used hierarchical Bayesian models to estimate the seed and seedling dispersal kernel for 24 of the most common tree species present at the Smithsonian forest research plot of Barro Colorado Island (Panama). For most of the species studied, the seedling densities did not peak away from the parent as predicted by the Janzen-Connell hypothesis, implying other mechanisms are necessary to control density and promote local diversity.

See a {{< staticref "uploads/pmarchand_esa2018.pdf" "newtab" >}}presentation{{< /staticref >}} and [publication](https://esajournals.onlinelibrary.wiley.com/doi/abs/10.1002/ecy.2926) on this project.

Photo credit: Christian Ziegler