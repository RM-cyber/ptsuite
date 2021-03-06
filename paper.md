---
title: 'ptsuite: An R-package for Fast Tail Index Estimation'
tags:
  - R
  - power law distributions
  - fat tailed distributions
  - heavy tailed distributions
  - pareto distributions
  - tail index
  - tail estimation
  - fast computation 
authors:
  - name: Ranjiva Munasinghe^[Corresponding author]
    orcid: 0000-0002-4059-8735
    affiliation: "1, 2" 
  - name: Pathum Kossinna 
    orcid: 0000-0002-4621-2557
    affiliation: 3
  - name: Dovini Jayasinghe
    orcid: 0000-0001-5685-3967 
    affiliation: 1
affiliations:
 - name: MIND Analytics & Management
   index: 1
 - name: Sri Lanka Institute of Information Technology
   index: 2
 - name: University of Calgary
   index: 3
date: 15 June 2020
bibliography: paper.bib


---

# Summary

Power law distributions, in particular Pareto distributions, describe data across diverse areas of study such as physics, astronomy, biology, economics and the social sciences. Real-world examples include distribution of wealth, word frequency in a given text, population in a city, stock market returns. In the present “Big Data” era, it is essential for programs to be optimized for speed and have the ability to handle large data sets. In particular, there are applications in genetics involving large data sets where power-law distributions describe network connectivity [@Zhang:2005]. We found some of the existing tail estimation packages in R are not optimized for speed especially when dealing with a large data set. The R-package `ptsuite` was developed to estimate the tail index for such (large) datasets with a focus on speed. In speed tests conducted, `ptsuite` outperformed similar R packages [@ptsuite:2020]. In addition `ptsuite` can 1) rapidly generate (large) Pareto data sets and 2) test if data is Pareto distributed. 

# About `ptsuite`

Features

1. Generate Pareto data (random variates)
2. QQ-plot (visual test for Pareto property)
3. Pareto Test (statistical test for Pareto property) [@Gulati:2008]
4. Various Tail Index Estimates (method classes listed below)
5. Function to generate Estimates using all methods 

Tail Index Estimation Classes [@Nair:2019; @Fedotenkov:2018]
 
1. Maximum Likelihood Methods
2. Least Square Methods 
3. Percentile Methods
4. Moment Estimators
5. Hill Estimators

The package `ptsuite` has been used in scientific publications [@Munasinghe:2019]. The authors plan to use it in forthcoming research and hope that it will assist other researchers and students with its combination of features, speed and ease of use.

The package `ptsuite` is available on Github: https://github.com/RM-cyber/ptsuite and Centralized R Archive Network (CRAN): https://CRAN.R-project.org/package=ptsuite. Further technical details (computational details, statistical background etc.), test results (accuracy of the estimates, speed comparison with other packages etc.) and other relevant information can be found in the R vignette [@ptsuite:2019] and ArXiv pre-print document [@ptsuite:2020].

# Acknowledgements

We wish to acknowledge Dr. J. Nair for helpful advice and in providing unpublished material for our research and Prof. S. Gulati for sharing knowledge on the Goodness of Fit tests. D. J. would also like to acknowledge Prof. S. Banneheka for a very useful discussion on the WLS method of estimation. 


# References
