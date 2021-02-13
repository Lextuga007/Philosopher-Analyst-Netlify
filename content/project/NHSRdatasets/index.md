---
title: "NHSRdatasets"
subtitle: "This is an overview of my contributions to this package."
excerpt: "An NHS package to help NHS, Public Health and related analysts/data scientists learn to use R"
date: 2020-04-23
author: "Zoë Turner"
draft: false
tags:
  - datasets
categories:
  - R
  - package
# layout options: single or single-sidebar
layout: single-sidebar
links:
- icon: door-open
  icon_pack: fas
  name: website
  url: https://cran.r-project.org/web/packages/NHSRdatasets/vignettes/ons_mortality.html
- icon: github
  icon_pack: fab
  name: code
  url: https://github.com/nhs-r-community/NHSRdatasets
- icon: newspaper
  icon_pack: far
  name: Blog post
  url: https://nhsrcommunity.com/blog/format-ons-spreadsheet/
---

![NHS-R Community](featured-hex.png)

### NHS-R Community [NHSRdatasets](https://github.com/nhs-r-community/NHSRdatasets) package is a package created to help NHS, Public Health and related analysts/data scientists learn to use R. It contains several free datasets, help files explaining their structure, and vignette examples of their use. 
---

### Contributing

This was the first time I contributed to a package and whilst I could produce a data set and write out a vignette in RMarkdown, I had barely used any GitHub. As with many things with the NHS-R Community, I had so much help from those in the community, notably from [Chris Mainey](https://www.mainard.co.uk/) and [Tom Jemmett](https://nhsrcommunity.com/blog/author/tomj/). 

I contributed a dataset of weekly provisionally recorded deaths in England from ONS from 2010 to 2019 and wrote out a [vignette](https://cran.r-project.org/web/packages/NHSRdatasets/vignettes/ons_mortality.html) of how I did this.

I also blogged about how the mortality data set was created for [NHS-R Community blog](https://nhsrcommunity.com/blog/format-ons-spreadsheet/) site.

### Evolution of the ons_mortality dataset

Since this has been released [The Health Foundation](https://www.health.org.uk/) have produced an API R package [{monstR}](https://github.com/HFAnalyticsLab/monstR) which accesses various datasets from the ONS, including weekly provisionally recorded deaths in England. I have written about how to access this data in a [blog](https://lextuga007.github.io/PhilosopherAnalyst/posts/2021-02-08-using-monstr-package/) and this is particularly useful as the data is more up-to-date and includes Covid deaths recorded from 2020.

My own code for creating the dataset changed too, and the code I used to extract the weekly provisional deaths includes extracting spreadsheet tabs, download a weekly changing url and now includes functions: [here](https://github.com/CDU-data-science-team/ONSDataCleansing/blob/master/R/mortality_ONS_2020.R). 

ONS also release monthly registered deaths which are more granular because the numbers are larger over a month. This isn't included in The Health Foundation {monstR} package and the [code I started](https://github.com/CDU-data-science-team/ONSDataCleansing/blob/master/R/mortalityMonthlyONS.R) is still a work in progress. There have been multiple changes to Local Authority names which need to be cleaned.  

### Using the mortality data

I've used the provisionally registered deaths information for a number of years as part of my trust's mortality surveillance. I use it in a [{dygraphs}](https://github.com/rstudio/dygraphs) chart that a Public Health Consultant colleague ([@IantheBee](https://twitter.com/IantheBee)) coded to show the similarity in patterns of death between the East Midlands and our trust mental and general health deaths. He used dygraphs so that it could have two axes but is also interactive. 

I wrote a blog on how to create this chart for the NHS-R Community [blogs](https://nhsrcommunity.com/blog/dygraphs/).
