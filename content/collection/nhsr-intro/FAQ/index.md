---
title: "Frequently Asked Questions"
weight: 12
subtitle: "Not necessarily frequently asked but definitely good questions"
excerpt: ""
date: 2021-05-12
draft: false
---


### Why does the course use the Cloud?

This has come up in courses but phrased differently as I sometimes have to explain things for the cloud and desktop as they differ. An major thing is when I explain projects in R Studio but the cloud _is_ projects so the demonstration needs to be on my computer and cannot be followed in the same way. 

The cloud is really useful to get around the different computer equipment that people have across the NHS, some of which don't support the latest R/RStudio and some have restrictions on what packages can be installed and it also means that all packages and files are installed and ready. Saying that, we've had problems with the cloud where people haven't had access (through restrictions on the VPN) or when the cloud is temporarily unavailable so there is no one perfect answer to this.

I try not to explain too much of how the cloud works because the purpose of the course is to try to get people started in RStudio on desktops but it does sometimes require some acknowledgement of difference, like that for projects, as the functionality is fundamentally different. 

### What packages would you recommend asking an IT department to install if there are strict rules around what can be installed?

Along with tidyverse and rmarkdown covered in this course other packages which could be useful are:

*CRAN packages*

* [NHSRdatasets](https://cran.r-project.org/web/packages/NHSRdatasets/NHSRdatasets.pdf) - of course I'd recommend this package! It's a package of datasets rather than functions but can be used in examples to share code with others. I use it a lot for mortality statistics in there for provisionally recorded weekly deaths from the ONS.
* [qicharts2](https://cran.r-project.org/web/packages/qicharts2/index.html) - for Statistical Process Control charts which also has great [vignettes](https://cran.r-project.org/web/packages/qicharts2/vignettes/qicharts2.html) are that clear and detailed. 
* [lubridate](https://lubridate.tidyverse.org/) - I suggested this when the question was asked and forgot it is already in tidyverse but is not covered in this course so is worth pointing out it's usefulness with handling dates.
* [janitor](https://cran.r-project.org/web/packages/janitor/vignettes/janitor.html) - cleans and helps exploring with Excel
* [datapasta](https://github.com/MilesMcBain/datapasta) - an addin for RStudio which allows the copying of data and pasting in a pre-formed layout like a data frame or vector.
* [beepr](https://www.r-project.org/nosvn/pandoc/beepr.html) - a package that makes a sound once code has run, which is immensely useful for slow running code that can then notify you if you switch between screens.
* [dataCompareR](https://cran.r-project.org/web/packages/dataCompareR/vignettes/dataCompareR.html) - for those that use data sets frequently where the question arises "this has changed but what is it precisely that's changed". I've used this to compare a dataset created in SQL and one in R to ensure the recoding has produced _precisely_ the same output.
* [PHEindicatormethods](https://cran.r-project.org/web/packages/PHEindicatormethods/PHEindicatormethods.pdf) - functions from Public Health Statistics including confidence intervals, rates, and DSRs

*Not on CRAN*

Other SPC packages that are good are 
* by John Mackintosh for [Run charts](https://github.com/johnmackintosh/runcharter) and [SPCs](https://github.com/johnmackintosh/spccharter)
* [fingertipsR](https://github.com/ropensci/fingertipsR) - a package to get Public Health England data as used in the [Public Health Profiles](https://fingertips.phe.org.uk/).

#### Do you have any suggestions on getting IT to approve installing R/RStudio?

I work for Nottinghamshire Healthcare NHS Foundation Trust which employs over 9,000 staff and allows anyone to install R and R Studio from an approved list. The Trust used to have licences for SPSS but revoked these due to cost and staff who used this statistical package are now expected to use R/RStudio and whilst some people have requested use of PSPP or Jamovi, these aren't on a global approved list in the Trust. 

Getting R/RStudio was only possible through the approval by our IT security team who and considers them, as do National bodies like NHSX, to be safe to install and use.

Whilst there is no one way to convince IT departments of the benefits of having R/RStudio and having the freedom to install packages with no restrictions I would say, try to ensure the request is with IT security and they know this is used elsewhere in the NHS. Showing people the benefits of R can help too as I show the work by [Trafford Data Lab](https://www.trafforddatalab.io/) as an example of publicly available data visualisations which would be of interest to Councils.

