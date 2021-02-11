---
title: "Create a Collection"
subtitle: "A collection, minus the blog."
description: |
  Sometimes you want a souped-up series- a bundle of related pages 
  meant to be read in sequence. This section is like a blog series, 
  minus the blog.
author: Alison Hill
show_post_thumbnail: true
show_author_byline: false
show_post_date: false
# for listing page layout
layout: list-sidebar # list, list-sidebar

# set up common front matter for all individual pages in series
cascade:
  layout: single-series 
  sidebar:
    title: "Bits and bobs"
    author: Zoë Turner
    description: |
        NHS-R Introduction to R and R Studio workshop slides. 
        The slides can be viewed here directly or expanded to full screen. 
        In the training I like to split my screen between the slides and live coding and the full screen doesn't work for that, so I use the GitHub pages that they feed from. The links can be found on the same page as the interactive slides.
        Slides have been converted to RMarkdown {xaringan} slides so resize within a web browser.
    show_author_byline: true
    show_post_date: true
    text_link_label: ""
    text_link_url: ""
    show_sidebar_adunit: true # show ad container, first page only
    text_series_label: "Outline" 
    text_contents_label: "On this page" 
---
