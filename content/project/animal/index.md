---
title: Animal Movement
summary: Fit individual-based models of animal movement to field data.
tags:
  - Ecology
date: ''
---

It is often useful to model biological or social systems by simulating the behavior of individuals based on set rules; so-called individual-based or agent-based models. For those models, forward simulation of the system is simple, but the inverse problem of inferring model parameters from observations is much more complex. This is due to each individual's path being the outcome of a series of decisions, each depending probabilistically on previous steps, so that a calculation of the likelihood across the "tree" of all possible paths becomes intractable. 

Approximate Bayesian computation provides a likelihood-free method to narrow down plausible parameter values in such models. A large number of simulations are performed from the model, each with a parameter set drawn from a broad prior distribution of the model's parameters. Then, the simulated outcomes that are sufficiently close to the observations in terms of key summary statistics are retained, and the parameter sets that produced them form the Bayesian posterior distribution of the parameters.

I have applied this method in different studies of animal foraging behavior. In one project, I compared the composition of pollen loads collected from bumble bees in a field to predictions from a simple efficient foraging model. The phenomenon of "floral constancy", where bees are observed to collect pollen from a single flower species in one foraging trip, could be explained simply by the fact that flowers of the same species tend to cluster in a field, and that efficient foraging trips focus on a small section of the field. ([Link to paper](https://www.sciencedirect.com/science/article/abs/pii/S0304380015002689))

For a different project, I modeled the day-to-day movement of radio-tracked toads along the shoreline of Lake Erie in Canada. The observations were best explained by a model where the toads randomly relocated each night (random walk), except that they had a fixed probability to return to a previous location; surprisingly, this probability did not depend on how far they had moved away from the previous location. ([Link to paper](https://www.sciencedirect.com/science/article/abs/pii/S030438001630850X)) ([GitHub](https://github.com/pmarchand1/fowlers-toad-move))

Photo credit: Morgan Boenke
