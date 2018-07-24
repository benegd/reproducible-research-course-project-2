---
title: "Reproducible Research Course Project 2"
author: "Benjamin Estrade"
date: "24 July 2018"
output: 
  html_document: 
    keep_md: yes
---

Synopsis
========














Project Goal
============

Use the data to answer some basic questions about severe weather events.

Questions:
1. Across the United States, which types of events (as indicated in the <span style="color:red" face="KaTeX_Typewriter">EVTYPE</span> variable) are most harmful with respect to population health?

2. Across the United States, which types of events have the greatest economic consequences?


Data Processing
===============

Details about project
---------------------

Copy of the data can be found in the [GitHub directory](https://github.com/benegd/reproducible-research-course-project-2).

Data retrived from the [here](https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2)

This project is part of the data science specialization course by John Hopkins University hosted by [Coursera](https://www.coursera.com/).

Consult README.md for more information




System info
-----------


```r
sessionInfo()
```

```
## R version 3.5.0 (2018-04-23)
## Platform: x86_64-w64-mingw32/x64 (64-bit)
## Running under: Windows 10 x64 (build 17134)
## 
## Matrix products: default
## 
## locale:
## [1] LC_COLLATE=English_Australia.1252  LC_CTYPE=English_Australia.1252   
## [3] LC_MONETARY=English_Australia.1252 LC_NUMERIC=C                      
## [5] LC_TIME=English_Australia.1252    
## 
## attached base packages:
## [1] stats     graphics  grDevices utils     datasets  methods   base     
## 
## loaded via a namespace (and not attached):
##  [1] compiler_3.5.0  backports_1.1.2 magrittr_1.5    rprojroot_1.3-2
##  [5] tools_3.5.0     htmltools_0.3.6 yaml_2.1.19     Rcpp_0.12.17   
##  [9] stringi_1.1.7   rmarkdown_1.10  knitr_1.20      stringr_1.3.1  
## [13] digest_0.6.15   evaluate_0.11
```


Downloading Data from orginal source
------------------------------------


```r
fileurl <- "https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2"
zippath <- "./ProjectData/Storm_data.csv.bz2"
projectdatapath <- "./ProjectData"
if(!file.exists(zippath)){
        if(!dir.exists(projectdatapath)){
               dir.create(projectdatapath) 
        }
        download.file(fileurl, zippath)
}
```






Results
=======












