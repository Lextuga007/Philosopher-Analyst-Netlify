---
title: "Prework"
weight: 2
subtitle: ""
excerpt: "How to prepare ahead of time."
date: 2021-02-07
draft: false
---

## Set up RStudio Cloud

Sign up for a free RStudio Cloud account at https://rstudio.cloud/ before the workshop. Log in with either an existing Google or GitHub account, or alternatively set up an account directly with RStudio Cloud.

NHS-R Community will send an email confirmation that will include the specific RStudio Cloud workspace invitation link. 

All the files and necessary packages are pre-loaded to the Cloud workspace.

When you first log in with the link shared in the email it will take you to an R Studio Cloud screen that says about Joining a space. Click on the blue button for Join Space:

![Screenshot of the workspace view in R Studio Cloud](rstudio-cloud.PNG)

The next screen that loads is a welcome page to the workshop (note that this screenshot is for the Shiny course):

![Screenshot of the welcome page after Join Space has been selected](welcome-to-workspace.PNG)

The final screen looks blank as it will say All Projects but nothing will be listed. If you click on the blue New Project this will start up the project that has all the necessary documents and packages all loaded. It can still take a few minutes to load:

![Screenshot of the Projects page which will be empty](project.PNG)

## If you want to use your own laptop/computer

Some VPNs (Virtual Private Networks) block access to RStudio Cloud or you may wish to use your own computer. VPNS sometimes do work but block parts of the R functionality, this is particularly a problem with Shiny apps (which is not covered in the Introduction to R and R Studio course).

If that is the case please ensure you have the **latest** [R](https://www.r-project.org/) and [RStudio](https://rstudio.com/products/rstudio/download/) installed. 

![A screenshot of a broken screen of smashed glass](broken.PNG)

It is important to have the latest R installed as older versions of R have had issues when installing tidyverse packages. Errors say that packages like `broom` or `readr` cannot be installed but even when this has been installed separately there continue to be other errors. Some of the [answers](https://community.rstudio.com/t/having-trouble-installing-and-loading-tidyverse-readr-no-hms-package/11268/7) in this post from RStudio community may help. 

If you require permission for programs to be installed on your computer and have got an older version of R and R Studio, it is worth asking for these to be updated by your IT department as this is always good practice for fixing known issues and bugs. 

### Packages

We will be using the packages {tidyverse} and {rmarkdown}, and whilst these packages are all available through CRAN and should be allowed by most organisations, if you have strict restrictions on what can be installed please have these approved or it may be better to use RStudio Cloud for the training.

`install.packages("tidyverse")` << This will be covered in the course itself
`install.packages("rmarkdown")`

##### October 2021

With the addition of slides and exercises for working with SQL databases, the following packages will also be required:

`install.packages(c("DBI", "dbplyr"))`


It's advisable to restart your R session before using any newly installed packages. Use the R Studio menu item *Session > Restart R* or the associated keyboard shortcut:

+ <kbd>Ctrl + Shift + F10</kbd> (Windows and Linux) or
+ <kbd>Command + Shift + F10</kbd> (Mac OS). 

## Course materials

#### Downloading files

If you plan to use the RStudio Cloud you can still download the following files, but it's not necessary for the workshop. 

If, however, you want to use your own computer go to https://github.com/nhs-r-community/intro_r_data and click on the green <kdb>Code</kbd> button

  ![Screenshot of the GitHub download files page with the selection from the dropdown of Download zip highlighted](github-download-files.PNG)
  
The zip includes the data files which will be used in the workshop. I have converted the slides to be published online (see below) and made a few updates to refresh the content. 

#### Using code to download files

If you want to use code to download all the files, open the zip file and create a project in R Studio to work from then the following package and code is needed:
  
``` r
install.packages("usethis")
usethis::use_course("nhs-r-community/intro_r_data")
```

## Downloading slides

If you want to have the slides on your computer, they can be downloaded from the same repository as the intro-r files but on a branch called [gh-pages](https://github.com/nhs-r-community/intro_r/tree/gh-pages). Using the same process as for `Downloading files` above you can download these to your computer by clicking on the green button and selecting the zip download.

#### Confirmation email

The NHS-R Community confirmation email will include: the link to the workshop, the RStudio Cloud workspace url and you should also receive a calendar invitation. If you are not sure that you can access zoom from your work laptop, please join a test zoom meeting coordinated by NHS-R Community.

#### Any problems

Please contact nhs.rcommunity@nhs.net if you have any issues.

#### Join the Slack group

A direct access link to the NHS-R Slack group will be shared in the workshop but the settings do allow some email addresses (like nhs.net) to sign up directly. The Slack url is [nhsrcommunity.slack.com](https://nhsrcommunity.slack.com/). Feel free to join the Slack group prior to the course!

There are channels for a wide variety of conversations including # help-with-r and # help-shiny. There is also a channel for # python and # book-club. 


Featured Art https://www.vintagevectors.com/objects/old-hot-air-balloons-and-blimps
and https://fixthephoto.com/broken-glass-overlay
