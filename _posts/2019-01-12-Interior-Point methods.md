---
layout: post
title: Interior-point methods from scratch
subtitle: A gentle introduction to primal-dual methods for linear programming
---

Over the past few decades, interior-point methods (IPMs) have become a standard and efficient tool for solving linear and non-linear optimization problems.
Their impressive performance stems from both strong algorithmic foundations and efficient numerical linear algebra.

This tutorial is a gentle and practical introduction to primal-dual interior-point methods for linear programming, illustrated with the implementation of an elementray IPM solver.
First, we introduce some core components of the theory underlying interior-point methods, and hint at their convergence properties.
Then, we discuss implementation aspects that make IPMs fast in practice, namely efficient linear algebra techniques.
Finally, we mention the extension of IPMs to non-linear optimization, and their use in the context of mixed-integer programming.

**Note**: No initial knowledge is required, other than elementary linear algebra.


## Outline

* [5-10min] High-level view of IPMs and simplex 
* [20min] The theory behind IPMs
  * Central path
  * Path-following algorithms
  * Hint at convergence properties
* [45-60min] Implementation
  * Mehrotra's predictor-corrector algorithm
  * Efficient linear algebra
  * Sparsity issues
* [10min] Beyond linear programming
  * Non-linear programming
  * Integer programming


## Implementation

The IPM solver will be coded in Julia, in the form of a fill-in-the-gaps exercise.
The initial code will contain instances from the Netlib library, the solver's squeleton as well as necessary utilities (e.g. instance reader) and data structures.

Missing parts, to be implemented during the tutorial,  include:
* Interior-point algorithm
  * Predictor and corrector directions
  * Step length
  * Stopping criterion
* Linear algebra
  * Normal equations system
  * Cholesky factorization (with Julia's standard library)

Other than basic knowledge of Julia and its LinearAlgebra library (which will be covered in the Julia tutorial), no advanced programming skills nor Julia knowledge are required.