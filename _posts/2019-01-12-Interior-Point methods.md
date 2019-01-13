---
layout: post
title: Interior-point methods from scratch
---

# Primal-dual interior-point methods for linear programming

Over the past few decades, interior-point methods have become a standard and efficient tool for 

This tutorial is aimed at a non-expert audience, and presents an overview of the core components of primal-dual interior-point methods for linear programming.

We introduce underlying theoretical concepts such as the primal-dual and barrier formulations, and the notion of central path. Practical aspects are also discussed, including linear algebra techniques and parallelization.

Finally, we point out the main pros and cons of interior-point algorithms, compared to the simplex method.

## Outline

* High-level view of IPMs and simplex
* Base theory
  * Central path
  * Barrier formulation
  * Path-following algorithms
* Implementation
  * Mehrotra's predictor-corrector algorithm
  * Efficient linear algebra
  * Sparsity
* Beyond linear programming
  * Non-linear programming
  * Integer programming