---
title: ‘ptsuite: An R-package for Fast Tail Index Estimation’
tags:
  - R
  - power law distributions
  - fat tailed distributions
  - heavy tailed distributions
  - Pareto distributions
  - tail index
  - tail estimation
  - fast computation 
authors:
  - name: Ranjiva Munasinghe^[Corresponding author]
    orcid: 0000-0002-4059-8735
    affiliation: "1, 2" 
  - name: Pathum Kossinna^[Author Without ORCID]
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

Power law distributions, in particular Pareto distributions, describe data across diverse areas of study such as physics, astronomy, biology, economics and the social sciences. Real-world examples include distribution of wealth, word frequency in a given text, population in a city, stock market returns. In the present “Big Data” era, it is essential for programs to be optimized for speed and have the ability to handle large data sets. In particular, there are applications in genetics involving large data sets where power-law distributions describe network connectivity [@Zhang:2005]. We found some of the existing tail estimation packages in R are not optimized for speed especially when dealing with a large data set. The R-package `ptsuite` was developed to estimate the tail index for such (large) datasets with a focus on speed. In addition `ptsuite` can 1) rapidly generate (large) Pareto data sets and 2) test if data is Pareto distributed. 

# About `ptsuite`

Features

1. Generate Pareto data (random variates)
2. QQ-plot (visual test for Pareto property)
3. Pareto Test (statistical test for Pareto property)
4. Various Tail Index Estimates (method classes listed below)
5. Function to generate Estimates using all methods 

Tail Index Estimation Classes
 
1. Maximum Likelihood Methods
2. Least Square Methods 
3. Percentile Methods
4. Moment Estimators
5. Hill Estimators

The package`ptsuite` has been used in scientific publications [@Munasinghe et al:2019]. The authors plan to use it in forthcoming research and hope that it will assist other researchers and students with its combination of features, speed and ease of use.

The package `ptsuite` is available on Github and Centralized R Archive Network (CRAN): https://cran.r-project.org/web/packages/ptsuite/index.html. Further technical details, test results (accuracy of the estimates, speed comparison with other packages etc.) and other relevant information can be found on the vignettes and ArXiv preprint documents.

# Computational Details

The technical specifications of the two computers used in the building and testing of this package are as follows: 

Laptop
CPU Intel(R) Core(TM) i5-8250U @ 1.60GHz, 1800 Mhz 
RAM 4 Core(s), 8 Logical Processor(s) 8GB 
OS Windows 10 Enterprise LTSC 10.0.17763 Build 17763 

Desktop
CPU Intel(R) Core(TM) i7-7700 @ 3.60GHz, 3601 Mhz RAM 4 Core(s), 8 Logical Processor(s) 32 GB OS Windows 10 Pro 10.0.17763 Build 17763 


Testing and development was done using R 3.5.2. and Microsoft R 3.5.1 [@MicrosoftTeam:2017] with the ptsuite 1.0.0 package. R itself and all packages used are available from the Comprehensive R Archive Network (CRAN) at https://CRAN. R-project.org/. Microsoft R may be obtained from https://mran.microsoft.com/ open. R Studio V 1.1.423 [@RStudioTeam: 2016] was used as the IDE for all tasks related to package development and generating results. The packages devtools [@Wickham et al B: 2018) and roxygen2 (Wickham et al A:2018) were used to assist in package documentation and development. The Rcpp package [@Eddelbuettel and François: 2011; @Eddelbuettel 2013; @Eddelbuettel and Balamuta: 2017] was used in the compilation of C++ code used in all estimation functions of the package. Finally
microbenchmark 1.4-4, ggplot2 3.0.0 [@Wickham: 2016] and plotly 4.8.0 were used in generating the results included in this paper. 


# Acknowledgements

We wish to acknowledge Dr. J. Nair for helpful advice and in providing unpublished material for our research and Prof. S. Gulati for sharing knowledge on the Goodness of Fit tests. D. J. would also like to acknowledge Prof. S. Banneheka for a very useful discussion on the WLS method of estimation. Financial support by MIND Analytics & Management.


# References
