---
author: KTamas
categories:
  - Uncategorized
date: 2013-01-26 13:35:42
guid: http://blog.ktamas.com/?p=2363369
id: 2363369
url: /index.php/2013/01/26/zene-kiszedese-youtubevideokbol-gyorsan-es-hatekonyan-nix-alatt/
permalink: /index.php/2013/01/26/zene-kiszedese-youtubevideokbol-gyorsan-es-hatekonyan-nix-alatt/
title: Zene kiszedése youtubevideókból gyorsan és hatékonyan *nix alatt
---

(Még mindig kósza posztok a draft mappámból)

Két dolog kell ahhoz, hogy gyorsan és hatékonyan zenét szedjünk ki youtubevideókból: [jwz](http://www.jwz.org) [youtubedown scriptje](http://www.jwz.org/hacks/youtubedown) és egy ffmpeg.

Az elsőt letöltjük, elrakjuk valahova, beállítjuk executablenek (`chmod +x`), berakjuk a `PATH`-ba és onnantól kezdve csak az URL-t kell hozzávágni, és szépen letölti az embernek az adott videóból a legjobb minőségű verziót. Aminek általában még így is szarrá van tömörítve a dynamic range-e, dehát mindent nem lehet.

Utána pedig _kimásoljuk_ a letöltött fájlból a hangsávot ffmpeg segítségével:
  
`ffmpeg -i youtubevideo.mp4 -acodec copy -vn zene.m4a`

A hang legtöbbször aac-ben van a videókban, ezért ad meg az ember m4a kiterjesztést a kimenetnek. Néha azonban nem, ekkor érdemes megnézni, hogy mi is van benne az `ffmpeg -i youtubevideo.mp4` segítségével.
