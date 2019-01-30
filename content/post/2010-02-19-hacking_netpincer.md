---
author: KTamas
categories:
  - Export
date: 2010-02-19 19:24:00
guid: http://ktamas.blog.hu/2010/02/19/hacking_netpincer
id: 1772778
url: /index.php/2010/02/19/hacking_netpincer/
permalink: /index.php/2010/02/19/hacking_netpincer/
tags: [netpincér, programozás]
title: Hacking netpincér
---

Van ehhez hosszabb háttérsztori is, de a lényeg az hogy kellett volna valami ami berendezi a netpincéren a szállítókat szállítási idő szerint. Ebből lett egy bookmarklet.

Egyelőre nem tudom, hogy lehet megcsinálni úgy, hogy ide is beilleszthessem, úgyhogy elkészíteni a következőképp lehet: [ennek az oldalnak](http://github.com/KTamas/netpincer_hacks/raw/master/netpincer_sortbydeliverydate.js) a tartalmát beilleszted [ide](http://javascriptcompressor.com/), majd az eredményt a vágólapra dobod.&nbsp;Csinálsz egy új bookmarkot, adsz neki egy hangzatos nevet, es a Location az lesz, hogy javascript:[a kód beillesztve ide]. Elmész a Netpincér oldalára, kiválasztod a szállítót, megnyomod a gombot, és ta-dám*, máris szállítási idő szerint vannak rendezve. Valahogy igy:

![](http://ktamas.blog.hu/media/image/netp.png)

&nbsp;

Amúgy a kód [fent van a githubon](http://github.com/KTamas/netpincer_hacks), tessék engem villázni. Lekódoltam azt is, hogy szűrni lehessen a boldogórás szállítókra de az azóta beépített fícsör lett. Remélem ez is az lesz egyszer.

*P.S.:&nbsp;Igen, a cuccnak kell kb. 2-3 masodperc lefutnia, mert a)&nbsp;betolti eloszor a jqueryt b)&nbsp;sajnos ki kell szednie es visszaraknia a DOM&nbsp;kb. felét amit a böngészők egyelőre nem viselnek jól. Ha valaki tud jobb megoldást, forkra fel.
