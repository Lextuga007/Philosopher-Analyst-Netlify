---
title: "Prework"
weight: 3
subtitle: ""
excerpt: "How to prepare ahead of time."
date: 2021-02-07
draft: false
---

## Equipment - screens

The course format is a shared screen of live coding with slides from the presenter to demonstrate coding. The opportunity to "code along" is encouraged and that may necessitate 2 screens for comfort of moving between the demonstration and using RStudio on your computer.

## Set up Posit Cloud

Sign up for a free Posit Cloud account at https://rstudio.cloud/ before the workshop. Log in with either an existing Google or GitHub account, or alternatively set up an account directly with Posit Cloud.

NHS-R Community will send an email confirmation that will include the specific Posit Cloud work space invitation link. 

All the files and necessary packages are pre-loaded to the Cloud work space.

When you first log in with the link shared in the email it will take you to an Posit Cloud screen that says about Joining a space. Click on the blue button for Join Space:

![Screenshot of the work space view in R Studio Cloud](rstudio-cloud.PNG)

The next screen that loads is a welcome page to the workshop and the final screen will have a project in it that is called `Intro_R_RStudio`. When this is selected the project gets copied so you will see both the original `Intro_R_RStudio` and your own new one called `Untitled`. Although the word `continue` appears next to the original screen you will open your copy.

## Difference between NHS-R workspaces and your own

You will be restricted to a certain [number of hours a month](https://posit.cloud/plans) on the free account which should be enough for the purpose of a day workshop, however, the NHS-R work space doesn't, currently, have that restriction. That may be changed in time and the work space will get cleared every so often though so if you need more time, get in touch with the nhs.rcommunity@nhs.net team for help.

## Taking the scripts to your own workspace

The NHS-R work spaces will get cleared every few months to keep them tidy and because access is based on a paid subscription. To move the project you've created to your own work space (which is available with the account you set up) select the moving trolley icon:

![Screenshot of the project name and to the right 4 icons, the bin for delete, moving trolley, the down arrow to download and three dots in a circle](select-icon-to-move.PNG)

Then select `Your work space`. If you've been invited to any other work space you will also see them in the same Move Content screen:

![Screenshot of the Move Content wizard with 3 options, Your work space and two others from NHS-R](move-content-menu.PNG)

It's possible to download your files instead by using the down arrow by the Project.

## If you want to use your own laptop/computer

Some VPNs (Virtual Private Networks) block access to Posit Cloud or you may wish to use your own computer. VPNS sometimes do work but block parts of the R functionality, this is particularly a problem with Shiny apps (which is not covered in the Introduction to R and R Studio course).

If that is the case please ensure you have the **latest** [R](https://www.r-project.org/) and [RStudio](https://rstudio.com/products/rstudio/download/) installed. 

![A screenshot of a broken screen of smashed glass](broken.PNG)

It is important to have the latest R installed as older versions of R have had issues when installing tidyverse packages. Errors say that packages like `broom` or `readr` cannot be installed but even when this has been installed separately there continue to be other errors. Some of the [answers](https://community.rstudio.com/t/having-trouble-installing-and-loading-tidyverse-readr-no-hms-package/11268/7) in this post from RStudio community may help. 

If you require permission for programs to be installed on your computer and have got an older version of R and R Studio, it is worth asking for these to be updated by your IT department as this is always good practice for fixing known issues and bugs. 

**Modern desktop users (NHS England)**

Some organisations are using a modern desktop system, please note that project do not appear to work with Projects/setwd and files like RMarkdown and Quarto don't appear to work, giving the error:

>Warning message:
>In options(stringsAsFactors = TRUE) :
>  'options(stringsAsFactors = TRUE)' is deprecated and will be disabled
>Error in setwd("C:/R/WorkingDir") : cannot change working directory
>Execution halted

Currently, the way around this is to create the missing folder "C:/R/WorkingDir" (so WorkingDir folder in a folder called R on the C: drive) and whilst the warning message will remain the report scripts `.rmd` and `.qmd` will work. The other recommendation is currently to work through UDAL if there is access.

### Packages

We will be using the packages {tidyverse} and {rmarkdown}, and whilst these packages are all available through CRAN and should be allowed by most organisations, if you have strict restrictions on what can be installed please have these approved or it may be better to use Posit Cloud for the training.

`install.packages("tidyverse")` << This will be covered in the course itself
`install.packages("rmarkdown")`

## Course materials

#### Downloading files

If you plan to use the Posit Cloud you can still download the following files, but it's not necessary for the workshop. 

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

The NHS-R Community confirmation email will include: the link to the workshop, the Posit Cloud work space url and you should also receive a calendar invitation. If you are not sure that you can access zoom from your work laptop, please join a test zoom meeting coordinated by NHS-R Community.

#### Any problems

Please contact nhs.rcommunity@nhs.net if you have any issues.

#### Join the Slack group

A direct access link to the NHS-R Slack group will be shared in the workshop but the settings do allow some email addresses (like nhs.net) to sign up directly. The Slack url is [nhsrcommunity.slack.com](https://nhsrcommunity.slack.com/). Feel free to join the Slack group prior to the course!

There are channels for a wide variety of conversations including # help-with-r and # help-shiny. There is also a channel for # python and # book-club. 


Featured Art https://www.vintagevectors.com/objects/old-hot-air-balloons-and-blimps
and https://fixthephoto.com/broken-glass-overlay
