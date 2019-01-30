---
author: KTamas
categories:
  - Uncategorized
date: 2012-10-28 17:50:24
fb-status-updater-meta:
  - a:5:{s:22:"custom-facebook-status";s:0:"";s:21:"custom-twitter-status";s:0:"";s:7:"fb-push";s:1:"1";s:7:"tw-push";s:1:"1";s:4:"push";s:1:"1";}
fb-status-updater-sn-reference:
  - a:2:{i:0;a:2:{i:0;s:8:"facebook";i:1;s:25:"722715145_430697956987186";}i:1;a:2:{i:0;s:7:"twitter";i:1;s:18:"2.625972280137E+17";}}
guid: http://blog.ktamas.com/?p=2363010
id: 2363010
url: /index.php/2012/10/28/pubsubhubbub/
permalink: /index.php/2012/10/28/pubsubhubbub/
title: PubSubHubBub
---

Egy újszülöttnek minden vicc új, mondják, de az megvan mindenkinek hogy a Feedburnerben egy klikkel be lehet kapcsolni a PubSubHubBubot (ami nincs bekapcsolva alapból, nem igazán értem, miért)? A Publicize -> PingShot alatt van a fícsör. És így nem fél nap alatt frissül a Google Readerben az adott feed.

Az persze másik dolog, hogy maga a Feedburner 10-20-30 perc delayyel dolgozik, ezt úgy lehet kiküszöbölni, hogy mi magunk is megpingeljük a Feedburnert, mikor a frissül a feedünk. Mióta a gugli megvette a szolgáltatást, azóta leginkább csak romlott, a dokumentációhoz vezető linkek például halottak, de [lehet találni](http://stackoverflow.com/questions/736413/ping-feedburner-in-django-app) példakódot. A végén [pár sor az egész](https://github.com/KTamas/sharewood.hu/blob/master/app/helpers/application_helper.rb#L3). Sőt, annyit kavartam hogy bekötöttem a [Superfeedr](http://superfeedr.com/)t is, úgyhogy one way or another mindenképp PuSHolva lesz a feed, realtime.
