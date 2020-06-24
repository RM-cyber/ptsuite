# `ptsuite`

R package `ptsuite` for fast tail index estimation for large datasets

![DOI](https://zenodo.org/badge/272910326.svg)](https://zenodo.org/badge/latestdoi/272910326)

GitHub: https://github.com/RM-cyber/ptsuite

C-RAN: https://CRAN.R-project.org/package=ptsuite 

**Instructions for Installation**

Following instructions are for Windows 64-bit operating system R for Windows version 3.6.0 

Requires RTools 

For R 3.6.0 use RTools version 35 https://cran.r-project.org/bin/windows/Rtools/history.html

Create a folder called .Renviron.txt in Documents folder  

```r
> writeLines('PATH="${RTOOLS35_HOME}\\usr\\bin;${PATH}"', con = "~/.Renviron")
> Sys.which("make")
 ## "C:\\rtools35\\usr\\bin\\make.exe"
```
Please modify accordingly for later versions of R and corresponding RTools version

To complete the installation
```r
>install.packages("devtools")
>library(devtools)
>install_github("RM-cyber/ptsuite", subdir="ptsuite")
```
