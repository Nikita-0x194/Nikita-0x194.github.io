---
layout: post
title:  "Creating a blog"
date:   2025-10-26 14:16:51 -0400
categories: jekyll update
---
## A Non-Coder's Battle with GitHub Pages and Jekyll

I started this blog as a way to capture the lessons and challenges I encounter on my journey through a career change. Mostly, I needed a place to jot down my thoughts and discoveries so they weren't simply floating around in my head.

A friend recommended GitHub Pages as the platform. I figured, "How hard can it be?" The simple answer: much harder than anticipated. Since I have absolutely no coding experience whatsoever, what I thought would be a quick setup turned into a multi-day ordeal.

## The Quickstart Dead End

My initial plan was simple: set up my existing GitHub account and enable Pages. I followed the [GitHub Pages Quickstart Guide][github-pages-quickstart] but immediately hit a wall. I realized I didn't have a _config.yml file, so I tried to create one manually via the GitHub web interface. I kept encountering things that were simply not part of my files. Like when the guide mentions to change this entry or that entry in the _config.yml file and mine is just blank. Now if I went through the creation process via ruby and bundle locally, the creation process makes defaults. That would have been a much better starting point. On the possitive, I learned it's exponentially better to use the local Command Line Interface (CLI) and Git, but after spending an entire evening fighting the web interface, all I had was a page that technically displayed something—but was utterly useless.

## The Jekyll Learning Curve

The next day, I knew there had to be a more efficient way. My research led me to the [About GitHub Pages and Jekyll][about-github-pages] documentation. Suddenly, I found myself installing Ruby, Jekyll, and Visual Studio on my desktop. I still didn't really understand the underlying technology, and the page never worked correctly. This was largely because I kept trying to change the theme without understanding how Jekyll themes are structured.

In this phase, I did manage a small victory: I learned the basics of Git: how to pull a repository, commit changes, and push them back up. However, a major complication was also trying to map my custom domain using a CNAME record, a process I struggled to connect between GitHub Pages and my domain provider.

## A Fresh Start in Linux

Frustrated with Visual Studio's interface, I decided to try again from the beginning in a Linux environment. I booted up a Pop!_OS virtual machine (VM) via Hyper-V, installed Ruby, and the required gems.

This time, I was determined to read a couple of different documentation guides before jumping into action. The single biggest goal I wanted to accomplish was being able to see the site locally before pushing any changes. I desperately needed to see the effects of my configuration edits in near real-time. This simple step has helped a ton in figuring out what each configuration setting actually does. I also learned that themes behave differently, so I’m sticking with the default for now while I build up my foundational understanding.

In summary, the quickstart guide led me astray, but the slow, frustrating process taught me about Git, changing configuration, and confirmed that I definitely prefer working in a Linux environment at the moment.

Here’s to many future "break-fixes" and the lessons they bring!

[github-pages-quickstart]: https://docs.github.com/en/pages/quickstart
[about-github-pages]: https://docs.github.com/en/pages/setting-up-a-github-site-with-jekyll/about-github-pages-and-jekyll
