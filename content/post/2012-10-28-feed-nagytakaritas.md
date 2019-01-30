---
author: KTamas
categories:
  - Uncategorized
date: 2012-10-28 17:40:08
fb-status-updater-meta:
  - a:5:{s:22:"custom-facebook-status";s:0:"";s:21:"custom-twitter-status";s:0:"";s:7:"fb-push";s:1:"1";s:7:"tw-push";s:1:"1";s:4:"push";s:1:"1";}
fb-status-updater-sn-reference:
  - a:2:{i:0;a:2:{i:0;s:8:"facebook";i:1;s:25:"722715145_481344588577220";}i:1;a:2:{i:0;s:7:"twitter";i:1;s:19:"2.6259464331579E+17";}}
guid: http://blog.ktamas.com/?p=2363178
id: 2363178
disqus_identifier: 2363178
url: /index.php/2012/10/28/feed-nagytakaritas/
permalink: /index.php/2012/10/28/feed-nagytakaritas/
title: Feed nagytakarítás
---

Leginkább note to self jellegű a bejegyzés, de hátha másnak is haszos lehet.

Az alapprobléma: nagyon sok feedet olvasok (587 jelen pillanatban), és szeretném tudni, nem-e változott meg valameliknek a címe / szűnt meg az oldal időközben.

A megoldás: végigmegyünk a feed URL-jein, és megnézzük, melik dob valami más HTTP státuszt, mint 200, ami ugye az OK.

Az eszközök: Ruby, Curl, valami posix-kompatibilis rendszer (Linux, OSX etc.)

Első körben letöltjük az OPML fájlunkat a readerből. Utána [ennek a ruby scriptnek a segítségével](https://gist.github.com/d2b82556b4c9bc5baddd) kiszedjük belőle az URL-eket a `subscription_urls.txt` fájlba.

Ezután [ez a script](https://gist.github.com/1ab093f30e4f6ad748f1) szépen végigellenőrzi a feedek HTTP státuszát (az outputot iranyitsuk tetszőleges szövegfájlba), végül nyissuk meg ezt a fájlt, és nyomjunk rá egy sortot kedvenc szövegszerkesztőnkben és indulhat a vadászat: minden ami nem 200-zal kezdődik, az gyanús.
