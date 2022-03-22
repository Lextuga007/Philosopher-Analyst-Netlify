---
title: "Prework"
weight: 1
subtitle: ""
excerpt: "How to prepare ahead of time"
date: 2022-02-10
draft: false
---

Due to issues that were reported by attendees at the first delivered course, the set up has changed. If there are any issues with using RStudio Cloud then own computers can be used, just copy the code for the packages and the data locally.

1. Learn about/refresh your knowledge of [Markdown](https://commonmark.org/help/tutorial/)

1. Sign up for a free RStudio Cloud account at https://rstudio.cloud/. Log in with either an existing Google or GitHub account, or alternatively set up an account directly with RStudio Cloud.

1. When in RStudio Cloud click on the blue `New Project` button in the top right of the screen and select `New RStudio Project`.

1. Install packages:

```r
install.packages(c("tidyverse", "rmarkdown", "here", 
                   "glue", "usethis", "distill", "bookdown",
                   "remotes", "shiny", "wesanderson"))
```

1. For the files copy the following into the console and run:

```r
usethis::use_course("Lextuga007/rm_01_basics")
```

# Notes on issues

## Shiny issue with `Knit with parameters...`

There are some issues with the course using the `Knit with parameters...` wizard in the RStudio Cloud as this uses the {shiny} package and may appear as a blank grey box. This may be related to VPN/Networks or some other security features of the organisation's equipment and may not be resolvable for the course but alternative ways of coding the use of parameters is covered in the section on Command Line.

## Internet browser

Please ensure that you use RStudio Cloud in either Chrome or Edge as Internet Explorer (which is sometimes default for NHS organisations) is not supported.
