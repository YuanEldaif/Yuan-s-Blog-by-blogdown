---
title: Publish blogdown website and deploy by Netflify
author: Yuan Du
date: '2019-07-09'
slug: publish-blogdown-website-and-deploy-by-netflify
categories:
  - R
tags:
  - Blogdown
  - Netflify
  - Github
---

I'm a noobie on using Github and Hugo. :blush: It took me quite a while to figure out how to use version control on Github through Rstudio. In this blog, I would like to share my hickhups on publishing website to Github and deploy my website by Netflify. Some of the hickhups were caused by not understanding the structure and logic of Github and the blogdown for configuration because I took a shortcut by googling and trials & errors and didn't feel like reading all the details of the Yihui's excellent [guidlines](https://bookdown.org/yihui/blogdown/). If you are really new user as me and want to use some tips, this hopefully should be very useful. You can skip some of the dump hickups that you hopefully not run into. You are very welcome to comment and help noobies like me improve.:pray:

Here are the hickups that I ran into on Github, Blogdown and Netlify:

- Make sure your R and Rstudio version is up-to-date. [Here](https://bootstrappers.umassmed.edu/bootstrappers-courses/courses/rCourse/Additional_Resources/Updating_R.html) you can find how to update R and Rstudio.

- Order of creating blogdown in Rstudio, github repo and Netlify

1. I highly recommend below order **before** you create blogdown as we have to use Github repo `<repo name>` to store all blogdown source files and deploy _public_ folder by Netlify.
    + Here is another order needed to pay attention. 
        + Click the _Clone or download_ green button and copy URL
        + In Rstudio terminal **Change** directory to Github repo you just created `<repo name>` by using `cd <repo name>`, 
        + Run `git clone <GitHub URL>` to clone new repository

2. Build your blogdown. I believe this step is easy to find. 
    + A tip to select multiple items to commit is by `git add .` and `git commit -m "your message"` and `git push origional master` in the terminal.
