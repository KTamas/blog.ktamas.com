---
author: KTamas
id: 1da1d4c45a7c63d9d191e539c37df15f
title: "In Memoriam of Sharewood — My Own Little Content Sharing Community"
date: 2019-01-15T09:56:04Z
lastMod: 2019-01-15T09:56:04Z
url: /index.php/2019/01/15/in-memoriam-of-sharewood-my-own-little-content-sharing-community/
permalink: /index.php/2019/01/15/in-memoriam-of-sharewood-my-own-little-content-sharing-community/
tags: [sharewood, rss, googlereader, writetogether]
type: post
draft: false
---
This post was inspired by the Motherboard article, [The Rise and Demise of RSS](https://motherboard.vice.com/en_us/article/a3mm4z/the-rise-and-demise-of-rss).

---

It was early 2012 and Google Reader's sharing function was taken from us, replaced with a useless, shitty "Share to Google+" button (Fuck you, Google). I've been using Reader since late 2006 and the sharing feature since it's introduction; the notion that if I see something interesting on the internet *I must share it with others* was ingrained in me, forever.

It started with conversations with friends, and we discovered that Posterous (RIP) had a decent bookmarklet one could use to grab content for sharing. So a few of us started content-sharing blogs (or linkblogs, if you will). Not long after, a friend suggested an idea: why don't we make our own content-sharing community? So we could use that for a back-end, all we need is a place where we aggregate all these blogs full of content.

The name of software that is used to aggregate RSS feeds is [Planet](https://en.wikipedia.org/wiki/Planet_(software)). There were and still are many Planet sites, so I went looking for a suitable engine, but none of them were right until I stumbled upon the [code](https://github.com/anildigital/planet) behind planetrubyonrails.com (RIP), written in, wait for it, Rails. I was already familiar with Rails, so [I forked it](https://github.com/ktamas/sharewood.hu), upgraded it to the latest version of Ruby on Rails, made a couple of changes and a basic design and by then I already had ten people interested, mostly from the old community at Reader.

A cronjob crawled the people's feeds, pulled the content into the database, stripped most of the formatting and then displayed it on the site, which itself had an RSS feed of course. And so, in early 2012, [Sharewood](http://goodbye.sharewood.hu/) (RIP) was born.

---

Over the next year or so our community has grown a bit. At the height of it, we had about 16 people. That may not sound like a lot, but a community is a community. People were sharing all kinds of interesting things, and I felt like I got back at least part of what we lost when Google neutered Reader.

The project was an opportunity for me as well to play with Rails; I ended up rewriting almost the entire codebase. I wrote a new RSS/Atom parser; tried to implement PuSH ([PubSubHubBub](https://en.wikipedia.org/wiki/WebSub)); added support for user accounts, so people would be able to follow others and get a custom RSS feed. I added a few tweaks to the front-end as well, like j/k navigation.

In early 2013 Google announced that they'd shut down Reader and a flurry of new alternatives appeared. One of the most promising ones was Hivemined, one that would never be finished; the one I ended up switching to was [NewsBlur](https://newsblur.com/) which I still use to this day. It's customizable, fast, has good support and UX. It also has built-in sharing and commenting support although it's not used widely. I tried switching to it, but never really got hooked on it, and I never had a community around it.

---

I shut down Sharewood in 2014, having done only basic maintenance on it for a year by then, and I felt like it has run its course.

My itch to share things is still very much present; I [maintain a Tumblr blog](http://sharing.ktamas.com/) where I share things irregularly, mostly webcomics I like. I also retweet interesting and funny things a lot [on Twitter](https://twitter.com/ktamas). But I still don't have a central place with a community like in the good old days, if you will.

I have no illusions; RSS will not make a comeback. Retweeting things and commenting on them or sharing things in private Slacks are as good as it gets right now.

The itch is still there.

*This post originally appeared on WriteTogether in [two](https://writetogether.space/posts/5/in-memoriam-of-sharewood-my-own-little-content-sharing-community-part-1-of-2) [parts](https://writetogether.space/posts/5/in-memoriam-of-sharewood-my-own-little-content-sharing-community-part-2-of-2).*
