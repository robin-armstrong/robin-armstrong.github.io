---
permalink: /projects/
title: "Projects"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## Structured Covariance Matrix Estimation

In joint work with [Anil Damle](https://www.cs.cornell.edu/~damle) and [Sam Otto](https://www.engineering.cornell.edu/faculty-directory/sam-otto) at Cornell, I am working to develop ultra-low sample complexity methods for estimating covariance matrices associated with forecasts or climatologies of high dimensional dynamical systems. This work draws on techniques from covariance localization and hierarchically rank-structured matrix compression.

For more information, please refer to this set of [slides](/files/slides_agu_2025.pdf).

## Numerical Methods for Data Assimilation

With [Ian Grooms](https://www.colorado.edu/amath/grooms) ([CU Boulder Dept. of Applied Mathematics](https://www.colorado.edu/amath/)), I developed an ensemble Kalman filtering algorithm which uses techniques from numerical quadrature and Krylov subspace iteration to update the ensemble from prior to posterior under a localized forecast covariance matrix. Compared to most existing methods, this algorithm achieves a more favorable trade-off between accuracy and cost when the system being modeled is extremely high-dimensional. With [Chris Snyder](https://www.mmm.ucar.edu/about/people/chris-snyder) ([NSF NCAR Mesoscale and Microscale Meteorology](https://www.mmm.ucar.edu/)), we have also been working to implement and test this algorithm on a full-scale forecasting problem using [MPAS](https://ncar.ucar.edu/what-we-offer/models/model-prediction-across-scales-mpas) and [JEDI](https://www.jcsda.org/jcsda-project-jedi).

For more information, please read our [preprint on arXiv](https://arxiv.org/abs/2503.00253), or this set of [slides](/files/slides_ds_2025.pdf).

## Efficient Matrix Factorization

With [Anil Damle](https://www.cs.cornell.edu/~damle) at Cornell, I developed an algorithm for efficiently computing column-pivoted QR (CPQR) factorizations of extremely large matrices. It is challenging to compute a CPQR factorization in a manner that takes advantage of BLAS-3 optimizations in core matrix-matrix products routines. Whereas most existing solutions to this problem target matrices with far more rows than columns, our algorithm targets the opposite situation: matrices with far more columns than rows. Matrices of this sort appear in scientific applications related to data clustering, model reduction, and computational chemistry. For a wide class of matrices arising in these domains, our algorithm runs significantly faster than the standard GEQP3.

For more information, please read our [preprint on arXiv](https://arxiv.org/abs/2501.18035), or these [slides](/files/slides_midatlanticna_2025.pdf). This work has also been submitted to the SIAM Journal on Scientific Computing.

## Fine-Grained Analysis of Interpolative Decompositions

Working with [Anil Damle](https://www.cs.cornell.edu/~damle) at Cornell and [Alex Buzali](https://seas.harvard.edu/person/alex-buzali), now at Harvard, I analyzed how the accuracy of interpolative decomposition algorithms for low-rank approximation are affected by the structure of the matrix being approximated. This work resulted in a set of theorems which describe the effects of subspace coherence and residual stable rank on interpolative decomposition approximation error, along with a comprehensive set of numerical experiments that compare several low-rank approximation algorithms across variations in relevant problem structures.

This work will soon appear in the SIAM Journal of Scientific Computing. You may also read our [preprint on arXiv](https://arxiv.org/abs/2310.09452) or this set of [slides](/files/slides_scan_2023.pdf).