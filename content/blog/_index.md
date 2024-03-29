---
title: Blogs
description: |
  Where I publish my thoughts is a little like my brain, it's in various places. This collects all of those places together.
author: "Zoë Turner"
show_post_thumbnail: true
show_author_byline: true
show_post_date: true
# for listing page layout
layout: list-sidebar # list, list-sidebar, list-grid

# for list-sidebar layout
sidebar: 
  title: Bibliotheca
  description: |
    Where I publish my thoughts and is a little like my brain in that my thoughts are all over the place. This page attempts to collect all of those places together.
    [Image](https://pixabay.com/users/nietjuh-2218222/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=3091212)
    
  author: "Zoë Turner"
  text_link_label: Subscribe via RSS
  text_link_url: /index.xml
  show_sidebar_adunit: true # show ad container

# set up common front matter for all pages inside blog/
cascade:
  author: "Zoë Turner"
  show_author_byline: true
  show_post_date: true
  show_disqus_comments: false # see disqusShortname in site config
  # for single-sidebar layout
  sidebar:
    text_link_label: View recent posts
    text_link_url: /blog/
    show_sidebar_adunit: false # show ad container
---

** No content below YAML for the blog _index. This file provides front matter for the listing page layout and sidebar content. It is also a branch bundle, and all settings under `cascade` provide front matter for all pages inside blog/. You may still override any of these by changing them in a page's front matter.**
