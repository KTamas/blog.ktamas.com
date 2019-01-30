---
author: KTamas
categories:
  - Export
date: 2009-01-26 09:43:08
guid: http://ktamas.blog.hu/2009/01/26/a_wind_es_az_ubuntu_esete_pt_1
id: 1769317
url: /index.php/2009/01/26/a_wind_es_az_ubuntu_esete_pt_1/
permalink: /index.php/2009/01/26/a_wind_es_az_ubuntu_esete_pt_1/
tags: [linux, ubuntu, wind]
title: A Wind és az Ubuntu esete, pt. 1
---

Szóval a hétvégén játszottam kicsit az Ubuntuval apám Windjén a <a href="http://wubi.sf.net" target="_blank">Wubi</a> segítségével és tulajdonképp nem volt rossz. Maga a rendszer 20 perc alatt felment sans letöltés, és majdnem minden hardvert azonnal felismert, es 5 perc google után megvolt a wifi is ami már-már scifibe illik. 

A legkisebb rossz jegyében a Gnome-ot választottam, a KDE4-et megnéztem a múltkor a winden és amellett, hogy lassú volt, usability szempontból szintén, khm, viszonylag hátul szerepelt a sorban. Gyorsan könnyes búcsút vettem az alsó taskbarszerüségtől (a futó programok felkerültek a felső menüsorra), majd felraktam a Gnome Do-t és kellemeset csalódtam: kiváló Quicksilver-klón, rakat pluginnal, és legalább annyira kézre áll. 

Elkezdtem ismerkedni a vimmel is, hála a vimtutornak, sőt, megcsináltam életem első .vimrc-jét is, meg felraktam a vim-ruby hogy legyen jó kis syntax highlighting, szóval <esc>:%s/mi az a vim/egész jó ez a vim/g. 

Az viszont nem menő, hogy az Intel videodriver apróbb hiányosságokban szenved még így 2009 tájékán is, például videolejátszás esetén <a href="http://en.wikipedia.org/wiki/Page_tearing" target="_blank">tearing</a> jelentkezik. Igazából látni kell, de olyasmi, hogy gyors mozgáskor a kép felső fele pár kockával előrébb jár, mint az alsó, és ezért eltérés van, ezért tearing, tehát szakadás. Létezik <a href="https://bugs.launchpad.net/ubuntu/intrepid/+source/xserver-xorg-video-intel/+bug/278318" target="_blank">részleges workaround</a> ami ezt elvileg kiküszöböli VLC meg MPlayer estén (átkapcsolni hardware overlayre), igaz ez is kicsit bugzik, ja és ez se nyújt megoldást pl. flash videó esetén, ami elég idegesítő. Elvileg a driver következő verziójába ez javítva lesz, amivel csak az a bajom, hogy ezt igérték a nemrég megjelent új verzióhoz is, csak aztán valahogy nem fért bele. Mindenesetre ez perpill _borderline dealbreaker_, mert a youtube-ról nem fogok lemondani. 

Ettől független lehet, hogy hamarosan beszerzek magamnak is egy ilyen kis gépet, főleg mert pl. a Windows 7 (is) nagyon jól fut rajta :)</esc>
