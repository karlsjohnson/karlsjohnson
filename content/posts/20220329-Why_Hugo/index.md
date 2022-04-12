---
title: "Why Hugo"
author: "Karl"
date: 2022-03-29T07:59:48+08:00
draft: false
tags: ["Website", "Hugo", "Markdown"]
categories: ["Computers"]
resources:
- name: "featured-image"
  src: "hugo_long.png"
description: "Switching to Hugo from Wordpress for my blog"

---

## Starting a Blog

After not blogging for many years, I wanted to write again. The purpose is to help collect my thoughts and record the technical skills I am learning. Writing about it makes it easier to remember. A blog also allows me to keep learning, whether it is technical or photography skills. I wanted something easy to use at first. I could always switch to something else later. Now, I have been writing with [Markdown](https://www.markdownguide.org/) for years. I much prefer it to MS Word or Apple Pages. It is also must easier to write websites in markdown compared to HTML. I tried several methods to set up a Markdown-based blog using [Static Site Generators](https://jamstack.org/generators/). All the ones I tried at first were difficult to set up, creating too many problems to run. So I tried to pick good old WordPress.

## WordPress

I set up a website with [Dreamhost](https://www.dreamhost.com/) and started configuring WordPress. It took a little while to learn and configure the theme, but I got everything working in a few days. I even had a Markdown plugin to write in Markdown instead of the standard editor. When that was all done, I started to write. I quickly found WordPress too slow, but I figured I could deal with it. The interface is also busy with lots of options. All of these options make the interface difficult to use. Even the Markdown interface was busy. After several posts, I could not stand how slow the whole writing process was. It took forever to start the interface, set up a post, paste the markdown, add pictures, and set up the post options. It was just too much of a barrier. So I had to change it and went looking.

![hugo_vs_wordpress](hugo_vs_wordpress.png "Hugo vs WordPress")

## Hugo vs WordPress

When I went looking for SSGs (Static Site Generators), I was trying to find javascript versions so I could learn javascript simultaneously. There are several nice javascript-based SSGs, but they are either difficult to understand or constantly updating and breaking. After much research, I picked [Hugo](https://gohugo.io/) and started playing around with it. It only took a day or two to choose a theme and set it up. I found the [LoveIt](https://hugoloveit.com/) theme had everything I wanted to start with. [Awesome-Hugo](https://github.com/theNewDynamic/awesome-hugo) is a good set of resources to learn more about Hugo. After a few days, I had Hugo set up on this site. It was much easier to set up and update with new content.

## Hugo Process

The process for creating a post will change in time, but it is already much faster than WordPress. I make a folder for each post, including an index markdown file and any images I want to include. Then I use [Typora](https://typora.io/) to write the post in markdown. I could use [VS Code](https://code.visualstudio.com/), but VS Code does not work with [Grammarly](https://app.grammarly.com/). Hugo also uses several extended Markdown features, but I will get into those in future posts. After writing the post, I add the images. I use a Bash Script to update Hugo's public directory and then rsync it to my  Dreamhost directory when the post is done. I don't even have to open a browser. 

## Learning Hugo

There is still a lot to learn about Hugo. Even with basic knowledge and I write and use it to create a Markdown blog and documentation site. I will be writing more as I learn how to develop more sites with Hugo.