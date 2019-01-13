---
layout: post
title: Interior-point methods from scratch
subtitle: A gentle introduction to primal-dual methods for linear programming
---

Over the past few decades, interior-point methods (IPMs) have become a standard and efficient tool for solving linear and non-linear optimization problems.
Their impressive performance stems from both strong algorithmic foundations and efficient numerical linear algebra.

This tutorial is a gentle and practical introduction to primal-dual interior-point methods for linear programming, and is illustrated by the implementation of an elementray IPM solver.
First, we introduce some core components of the theory underlying interior-point methods, and hint at their convergence properties.
Then, we discuss implementation aspects that make IPMs fast in practice, namely efficient linear algebra techniques.
Finally, we mention the extension of IPMs to non-linear optimization, and their use in the context of mixed-integer programming.

**Note**: No initial knowledge is required, other than elementary linear algebra.

## Outline

* High-level view of IPMs and simplex
* The theory behind IPMs
  * Central path
  * Path-following algorithms
  * Convergence properties
* Implementation
  * Mehrotra's predictor-corrector algorithm
  * Efficient linear algebra
  * Sparsity issues
* Beyond linear programming
  * Non-linear programming
  * Integer programming

## Implementation notes

The IPM solver will be implemented in Julia. Other than basic knowledge of Julia and its LinearAlgebra library, no advanced knowledge is required.