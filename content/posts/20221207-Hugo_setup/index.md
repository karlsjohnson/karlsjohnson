---
title: "Setting up Hugo"
author: "Karl"
date: 2022-12-07T00:00:00+06:00
lastmod: 2022-12-07T00:00:00+06:00
draft: false
resources:
- name: "featured-image"
  src: "featured-image.jpg"
tags: ["Hugo, CLI"]
categories: ["Website"]
description: "Hugo Setup"
---

## Setting up Hugo

After 8 months, I am back posting on my website. Hopefully more will follow. I will be updating this post over the coming days to document my current setup for this website. This post will be about my setup process for this blog or any other [hugo](https://gohugo.io/) website.

<!--more-->

## Requirements

I am using [hugo](https://gohugo.io/installation/macos/) installed on the mac. KNowledge of the command line will be required. I use [homebrew](https://brew.sh/) for installing command line programs and that is also required. Follow the link to learn how to install. It is pretty easy with the one line command. [Git](https://formulae.brew.sh/formula/git#default) should also be installed on your system with brew.

I am using the [LoveIt](https://hugoloveit.com/) theme for my site. The Loveit theme has pretty of markdown options for adding code, math, and more. The repository fo this theme is [here](https://github.com/dillonzq/LoveIt).

## Installing

To install hugo on the mac, use homebrew install command

```bash
brew install hugo
```

## Creating a new site

Following the [quick start](https://gohugo.io/getting-started/quick-start/) would be good to foloow to understand the basic usage of hugo. The main commands are the following:

To create a new project or website:

```bash
hugo new site name_of_project
```

Initialize an empty Git repository for project:

```bash
cd name_of_project
git init
```

Clone the Loveit theme into the themes directory, adding it to your project as a Git submodule. Then add the theme to your config file.

```bash
git submodule add https://github.com/dillonzq/LoveIt.git themes/LoveIt
echo "theme = 'Loveit'" >> config.toml
```

Run hugo as a server. Hugo will server the new project [here](http://localhost:1313/). Press Ctrl + C to stop Hugo’s development server.

```bash
hugo server
```

To Build the project into a folder 'public' that will be inside your project folder run the following command. you can sync/copy the public folder to your host.

```bash
hugo
```

## Configure the site
