---
title: "Frequently Asked Questions"
weight: 2
subtitle: "Not necessarily frequently asked but definitely good questions"
excerpt: ""
date: 2022-03-18
draft: false
---

### Who should attend?

No prior knowledge of R is required; however, it is assumed that you will have a moderate level of computer literacy. For example, you will be able to navigate to drives and files and be confident in searching for solutions to technical problems on the internet. You will work with, or have an interest in, data. 

### Why R?

R is one of the most powerful data science software solutions used the world over and is being actively promoted by the NHS-R Community. Analysts throughout the NHS and in Social Care are discovering the huge potentials of R which range from analytical and statistical work to creating websites and interactive reports. It’s a hugely flexible and versatile language that has far extended its original use for statistics.

### What are the Learning Outcomes for the course? 

After this one-day introduction, you will:

1.	See examples of R in producing healthcare related visualisations and use publicly available healthcare data to answer questions.  
1.	Recognise and understand key terms often used by users of R. 
1.	Interact with R using the RStudio environment.
2.	Learn how to set up some of the accessibility features of RStudio. 
1.	Take charge of their workflow using RStudio projects.
1.	Import data into R using csv files (other data sources will be discussed).
1.	Carry out data manipulation using simple steps to solve complex problems.
1.	Join multiple tables together.
1.	Produce and save plots using ggplot2.
1.	Learn how to find more information on functions within R packages.
1.	Open an RMarkdown template and learn how to get started in producing an integrated text and code report.
1.	Take away ideas for continuing learning after the course.

### What is the agenda?

Timings in the course vary depending on any issues that people may encounter.

*Using R Studio*
Some examples of the use of R and how to set up R Studio  

*Using Projects*
How and why to use projects in R Studio

*Importing data*  
How to use the import wizard in R Studio and try importing example Excel spreadsheets  

--------- Break ---------  

*Introduction to ggplot2*   
An introduction to ggplot2 and plotting data  

*What does this function do?*  
How to locate help functions  

--------- Lunch -----------  

*Data wrangling with dplyr*  
Introducing a few of the key dplyr functions to help shape and tidy data  

*Naming objects* 
How to create an object from some code or a plot  

--------- Break ---------  

*Relational data*  
How to join data using dplyr  

*R Markdown*  
Introducing RMarkdown reports  

*Ongoing learning*  
Suggestions for further R resources  


### Where is the code that built this?

Currently, the code that built the site can be found in the [Philosopher Analyst](https://github.com/Lextuga007/Philosopher-Analyst-Netlify/tree/main/content/intro-r) Hugo Apéro site.

The code for the slides themselves is hosted on the [NHS-R Community GitHub repository](https://github.com/nhs-r-community/intro_r) which is broken down into several parts, the slide code, the html output and the data files used in the course. See the repository for links.

### I'm interested in training this course where can I find more?

I recently did a Train the Trainer event for the NHS-R Community and [compiled information](https://philosopher-analyst.netlify.app/talk/nhsr-train-the-trainer/) including the recorded workshops from the conference. We also have a particular channel in the NHS-R Slack group called #training where we discuss who can do what training for the community. We are always looking for trainers and supporters to assist in the training so do get in touch through [Slack](nhsrcommunity.slack.com) or [contact me](https://philosopher-analyst.netlify.app/contact/).

### Slides/RStudio/GitHub doesn't show or work

Often problems with the slides not showing, RStudio Connect not loading and GitHub losing functionality is due to being on a VPN (Virtual Private Network)/Network. My Trust, for example, does not allow RStudio Connect and whilst I can view GitHub, I'm not able to do some things like download zip files. 

To download the html files to work offline or off a VPN/Network go to the [NHS-R Community GitHub Repository](https://github.com/nhs-r-community/intro_r/tree/gh-pages) and click on the green button `Code` to download the zip file. As these slides are built using {xaringan} the zip file contains folders `css`, `libs` and `img` which the slides needed to be created but which are not needed if you are looking at them locally. They are `self-contained` so you can delete these folders with no impact on the slides.

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


#### How long does it take for someone with no coding experience to learn R?

This was a great question that really resonated with me as I firmly believe that anyone who wants to learn R can. Having another language beforehand can often help but it can also be a hindrance, it really depends on the person or the problem you are working on. I've heard it's possible to learn R in a week with the right support but it feels too much putting an expectation saying time scales like this as people learn at different rates. It also depends what is meant by 'knowing R' as I really enjoy tidying data and picked that up quickly but I'm very slow at coding a chart and I would take an age to do a map! 

If you want to learn R, you can, and you will succeed the best way that suits you in the time that's right for you. But remember there is a great community using R who are also want you to succeed and there's no better place than the NHS-R Community Slack group: nhsrcommunity.slack.com. I've asked plenty of questions there that may have been 'simple' but this is a supportive space 
where there is no question that is too simple.

#### Tips on practicing R after the course.

In the course I fully acknowledge that it's incredibly hard to always use R for projects when you first start out, particularly with any time pressures to complete tasks. I found it very difficult when I first started, and would often defer back to the tools I knew I could use quickly (namely SQL and R). However, we know the best way to learn anything, including languages, is to practice and use it. 

I suggest either trying a project that doesn't have these time pressures, but is interesting enough that you want to solve it, or replicate something that you've already done. For example, reproducing a statistical test, tidying a dataset or reproducing a chart. Doing this can take time but takes some pressure of needing to complete it as it already exists and then you are also able to make comparisons which can be useful for statistics or data cleaning. 

#### How can I practice using R if I don't have projects/analyst work that is suitable?

This particular question was posed by someone who also doesn't necessarily use quantitative data so they wanted to know how they could keep up their learning. This was a great question to showcase some of the R projects that people can get involved with and a few are listed here:

* NHS-R Community projects on [GitHub](https://github.com/nhs-r-community) are perfect for getting involved with the community, even for those just starting out with using R. There are many and varied projects but you also don't necessarily need to code to contribute. Lots of projects need people to test out the vignette code, ask questions, write out things like Code of Conducts. There is always help too with these projects which are often coordinated through the NHS-R Slack group.

* [Tidy Tuesday](https://github.com/rfordatascience/tidytuesday) is a weekly data project in R that you can join in exploring a dataset, visualising it and also get to see how others work on the data through the hashtag #TidyTuesday.  

* Reading the [R for Data Science](https://r4ds.had.co.nz/index.html) book is great as it includes exercises that use the pre-loaded cars dataset. The [unofficial answers](https://jrnold.github.io/r4ds-exercise-solutions/) is also very useful and interesting as it both gives the solution and expands on the concepts. The [NHS-R Book group](https://github.com/nhs-r-community/book_group) is also (as of December 2021) reading through this book.

* Consider setting up your own blog/website. There are two very fun ways to build sites in R: [distill](https://rstudio.github.io/distill/) and [Hugo Apéro](https://hugo-apero-docs.netlify.app/learn/). I've also built [a template in {distill}](https://github.com/CDU-data-science-team/distill-blog-template) for the CDU Data Science Team that may be helpful to also get started.

Many people use these sites to quickly build and collate their projects together and they can be incredibly inspirational. Showcase examples include:

- [distill's examples](https://pkgs.rstudio.com/distill/articles/examples.html)
- [distillery showcase](https://distillery.rbind.io/showcase.html)
- [R-Ladies's collated blogs](https://github.com/rladies/awesome-rladies-blogs)
- [Hugo Apéro's showcase](https://hugo-apero-docs.netlify.app/project/)

Sites don't have to be about coding as I've built a site to put together all the information I was collating about Ethics for the [Ethics Committee](https://ethics-committee-resources.netlify.app/collection/) at my Trust. You can use your own pictures or those that are [free](https://github.com/jennybc/free-photos) and have a lot of fun being creative with R. I'd recommend just ensuring that all images have a CCO licence and try to include a credit somewhere. That's good for the original owner but also useful for you too when you want to retrace where you located the image.

## Explaining a boxplot

It's possibly because I get very excited in the course about boxplots that it's reasonable for people to ask about them! One of the best explanations I've seen is by Simon Wellseley-Miller from the [AphA conference in 2021](https://www.youtube.com/watch?v=rsFh0MPZra8) at 0:51 on understanding Length of Stay using boxplots. The presentation slides are available on the [AphA website](https://www.aphanalysts.org/documents/presentations-day-1-2/).

