---
author: KTamas
id: 1687895b53d3646b4c5897d4bd92db12
title: "Converting My Blog To Hugo and Getting Rid of My VPS"
date: 2019-02-01T11:46:09Z
lastMod: 2019-02-01T11:46:09Z
url: /index.php/2019/02/01/converting-my-blog-to-hugo-and-getting-rid-of-my-vps/
permalink: /index.php/2019/02/01/converting-my-blog-to-hugo-and-getting-rid-of-my-vps/
tags: [meta, tech, hugo, writetogether]
type: post
draft: false
---
[I have a blog](https://blog.ktamas.com) (you're reading it!). It's got history: I set it up in early 2009, and I have almost 600 posts, mostly in Hungarian. I had one before that, between 2005 and 2008, but it was lost due to a variety of reasons, including my failure to properly back things up. Small bits of it are still [up in the Wayback Machine](http://web.archive.org/web/20070208165650/http://blog.ktamas.com/), though. It was all in Wordpress, which does its job, though even in 2019 it can be a pain to update things.

### From Wordpress to Jekyll to Hugo

About a week ago I decided it was time to migrate it to [Jekyll](https://jekyllrb.com/). I was bored, and it gave me a good excuse to play with a static site generator. Plus, doing this kind of conversion became a rite of passage for people working in tech these days.

*This is not a complete guide; you can find hundreds of them with a [quick google](https://www.google.com/search?q=convert+wordpress+to+jekyll). I will, however, provide a general overview of the process with some helpful pointers and links.*

I started by migrating all the comments to Disqus with their [official Wordpress plugin](https://wordpress.org/plugins/disqus-comment-system/). After that, I used a [Jekyll exporter plugin](https://wordpress.org/plugins/jekyll-exporter/) that converted all my posts into markdown... except it stripped all the embeds.

I used to blog a lot about music, so I had a lot of embeds, mostly from Youtube. In retrospect, I could have saved myself some time by patching the exporter or finding another one. In the end, however, I ended up fixing every single post by hand. I replaced old, pre-iframe flash embed codes with updated ones and changed the newer, but still http ones to https. In most places, if the video was not necessary or wasn't available anymore, I added the song to the post via Spotify. The chances of a given song being up on Spotify in a few years feels *marginally* higher than on Youtube right now. I had a few other embeds that I could fix with newer code (Soundcloud) and others that I couldn't (Deezer), but most of the time I could find the given song or playlist within Spotify. All of this had the benefit of walking down on memory lane, reading 10-year old blog posts and cringing a lot. *I was so young.*

---

I've found a [reasonably decent theme](https://github.com/vinitkumar/white-paper) for Jekyll, which felt like a good starting point, though it didn't have built-in support for tags or archives. I started googling how to implement that, and around the same time I was venting about my embed issues on the XOXO slack. That was when [David](https://twitter.com/theory) chimed in about his experiences on doing this exact same process, except he ended up using [Hugo](https://gohugo.io), another popular static site generator that's kind of like Jekyll except faster. [The theme](https://github.com/theory/justatheory/tree/master/themes/justatheory) of [his blog](https://justatheory.com) had everything I wanted: a fancy archives page and proper support for tags. So I figured I might as well continue my journey: switch to Hugo and use his theme as a basis.

Jekyll is written in Ruby and uses a simple templating language. Hugo's code is in Go, and it uses Go's own templates; they definitely have a learning curve, even if you have coded in Go before. With some help, googling and a lot of trial and error, I got the hang of it and managed to change things to my liking as well as the look and the color scheme of the site. I converted most of my posts' [front matter](https://gohugo.io/content-management/front-matter/) [with a script](https://github.com/coderzh/ConvertToHugo) and fixed the rest with a few search-and-replaces. With 8-10 hours of work behind me — half of that was fixing those embeds — I had my new blog ready to be [hosted on Github Pages for free](https://pages.github.com/). I use a modified version of the [sample deploy script](https://gohugo.io/hosting-and-deployment/hosting-on-github/#put-it-into-a-script-1) they have in Hugo's documentation. 

### Getting Rid of My VPS

I had a small VPS at Linode for years now, hosting my pet projects, my blog and a bunch of static sites (like my [home page](https://ktamas.com)) over the years. It also had OpenVPN installed so I could watch iPlayer for free until BBC started cracking down on that. By now it only had my blog and those static sites; I figured if I could find something for the latter, I could ditch the VPS entirely.

I don't remember how, but I came across [Netlify](https://netlify.com). They give you free static hosting with extremely generous soft limits (100 gigs of storage, 100 GB/month transfer). You just point them to a Github repository, and about 30 seconds later you have your site ready, with support for multiple custom domains and SSL.

I spent an hour or two moving everything to Netlify, changing the necessary DNS entries and in the end, I was ready to say goodbye to my VPS and save a grand total of $7 a month in the future. I made backups of everything and then, somewhat emotionally pressed the "Delete" button on Linode's control panel. I wouldn't be surprised if I would get another one eventually for a side project or something, but for now, I'm happy with my all my stuff hosted around the internet for free and stored in git repos.

### On the Future of My Blog

Making this move also means that I will start cross-posting my posts from [WriteTogether](https://writetogether.space/users/ktamas) to here. One-off posts like this one will definitely make it here; the ongoing series I have at WriteTogether will probably stay there until they are done, and then I'll re-edit them into long-form posts and publish them here. I will also post content here that doesn't fit WriteTogether for one reason or another. Feel free to [subscribe to this blog](http://feeds.feedburner.com/KTamasBlog) in your favorite RSS reader.

Hugo gives me a lot of ways to tinker; I am already thinking about replacing the commenting system, adding reading time, word count and so on. I might write something on this in again in the future.

*This post was not sponsored by anyone, just in case some of it reads like an ad for Github or Netlify or whatever.*

*This post originally appeared on [WriteTogether](https://writetogether.space/posts/ktamas/converting-my-blog-to-hugo-and-getting-rid-of-my-vps).*
