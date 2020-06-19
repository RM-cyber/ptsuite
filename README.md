# `ptsuite`

R package `ptsuite` for fast tail index estimation for large datasets


Available at

GitHub:https://github.com/RM-cyber/ptsuite

C-RAN: https://CRAN.R-project.org/package=ptsuite 

Instructions for Installation

For Windows 64-bit operating system R for Windows version 3.6.0 

Requires RTools 

For R 3.6.0 use RTools version 35 https://cran.r-project.org/bin/windows/Rtools/history.html

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
