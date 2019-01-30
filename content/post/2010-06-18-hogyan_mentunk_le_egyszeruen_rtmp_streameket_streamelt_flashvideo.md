---
author: KTamas
categories:
  - Export
date: 2010-06-18 21:49:39
guid: http://ktamas.blog.hu/2010/06/18/hogyan_mentunk_le_egyszeruen_rtmp_streameket_streamelt_flashvideo
id: 2092556
url: /index.php/2010/06/18/hogyan_mentunk_le_egyszeruen_rtmp_streameket_streamelt_flashvideo/
permalink: /index.php/2010/06/18/hogyan_mentunk_le_egyszeruen_rtmp_streameket_streamelt_flashvideo/
title: Hogyan mentunk le egyszeruen RTMP streameket (streamelt flashvideo)
---

Amolyan jegyzet magamnak, meg hatha megtalalja egyszer valaki guglibol. Hozzavalok egy linux, amin van iptables es sudo, meg az rtmpdump leforditasahoz szukseges dolgok (ubuntun ez a build-essential csomag).

  * [Leszedjuk az internetrol](http://rtmpdump.mplayerhq.hu/download/) az rtmpdumpot, kicsomagol, configure script nincs, make, sudo make install.
  * Hozzaadunk egy tetszoleges felhasznalot `sudo adduser rtmpsuck`
  * Atiranyitjuk az rtmp forgalmat az iptables-szel:&nbsp;`sudo iptables -t nat -A OUTPUT -p tcp --dport 1935 -m owner &nbsp;\! --uid-owner rtmpsuck -j REDIRECT`
  * Atlepunk a felhasznaloba `sudo su rtmpsuck`
  * elinditjuk az rtmpsrv-t egy olyan konyvtarbol, amihez van irasi joga
  * elinditjuk a bongeszot, abban pedig a lejatszast, es mar menti is le szepen.
