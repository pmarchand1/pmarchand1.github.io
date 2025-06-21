---
title: rslurm
summary: R package to submit calculations to a 'Slurm' cluster.
tags:
  - Software
date: '2025-06-21'
---

The [rslurm](https://www.earthdatascience.org/rslurm/articles/rslurm.html) package simplifies the process of executing a R function in parallel over a range of inputs, for computing clusters that use the Slurm workload manager. Its main functions use a syntax similar to well-known R commands for the distributed evaluation of a function (the 'apply' family of functions). They automatically divide the computation over multiple nodes and write the necessary submission scripts in Bash. The package also includes functions to retrieve and combine the output from different nodes, as well as wrappers for common Slurm commands.

I was the original main author of the package, which is now being maintained by the University of Colorado Boulder's Earth Lab ([GitHub](https://github.com/earthlab/rslurm)).
