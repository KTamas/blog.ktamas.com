---
author: KTamas
categories:
  - Uncategorized
date: 2012-08-07 13:19:22
fb-status-updater-meta:
  - a:5:{s:22:"custom-facebook-status";s:0:"";s:21:"custom-twitter-status";s:0:"";s:7:"fb-push";s:1:"1";s:7:"tw-push";s:1:"1";s:4:"push";s:1:"1";}
fb-status-updater-sn-reference:
  - a:1:{i:0;a:2:{i:0;s:7:"twitter";i:1;s:19:"2.3279809238521E+17";}}
guid: http://blog.ktamas.com/?p=2363190
id: 2363190
url: /index.php/2012/08/07/rdp-osx-alatt/
permalink: /index.php/2012/08/07/rdp-osx-alatt/
tags: [commandline, mac, osx]
title: RDP OSX alatt
---

Valószínű nem én vagyok az egyetlen, akinek a munkája miatt be kell RDP-znie különböző Windowsos gépekre &#8212; és OSX-et használ. 

A rendes felhasználó természetesen először a hivatalos megoldással próbálkozik, a Microsoftnak van egy [Remote Desktop Connection Client](http://www.microsoft.com/mac/remote-desktop-client) nevű szoftvere, letölt, felrak, minden megy. Kivéve persze, hogy nem, mert [másfél éve nem frissült](http://www.microsoft.com/mac/downloads?pid=Mactopia_RDC&fid=68346E0D-44D3-4065-99BB-B664B27EE1F0#viewer), és már 10.6 alatt is szeretett kifagyni pl. kilépéskor, 10.7 alatt még instabilabb lett, most így 10.8-ra már fel se rakom. Arról nem is beszélve, hogy például csak egyetlen fix felhasználónév-jelszó-domain triót tud megjegyezni, és ha megjegyeztetjük vele, akkor az összes szervernél ezzel fog próbálkozni. Szóval ez az opció sajnos kiesik, és az ember elkezd alternatívákat keresni.

Valószínű gyorsan beleakad a [CoRD](http://cord.sourceforge.net/)-ba, ami bár egy remek szoftver, van egy hatalmas hibája: a háttérben az [rdesktop](http://en.wikipedia.org/wiki/Rdesktop) nevű projektet használja, ami viszont nem tudja hozni a hivatalos kliens sebességeit, egyszerűen lassabb, és emiatt lényegesen kényelmetlenebb.

A &#8212; szerintem &#8212; igazi megoldás pediglen a [FreeRDP](https://github.com/FreeRDP/FreeRDP). Ez a már fentebb említett rdesktop projekt egy forkja. GUI sajnos nem jár hozzá, cserébe működik, és gyors. Felrakni legegyszerűbben a homebrew-n keresztül lehet, `brew install freerdp` és utána máris elérhetővé válik az xfreerdp parancs. Azért X, mert X11-et használ, amit az Apple száműzött a Mountain Lionból, de _fear not_, [innen](http://xquartz.macosforge.org/landing/) le lehet tölteni és felrakni, és újra van X-ünk.

Az `xfreerdp --help`ből nagyon gyorsan meg lehet találni, milyen paramétereket kell megadni a kapcsolódáshoz, az egyetlen dolog amit kicsit keresnem kellett, az a vágólap-szinkronizáció, ami &#8212; és még pár egyéb funkcionalitás, érdemes elolvasni [ezt](http://linux.die.net/man/1/xfreerdp) &#8212; valamiért ki van szervezve egy külön pluginba, ezért azt külön be kell vele töltetni vele. Én írtam magamnak egy nagyon egyszerű *sh funkciót, bevágtam a .zshrc-mbe (de ugyanúgy megy bashből is, egyébként), így néz ki:

`function rdpw() { xfreerdp -u $1 -p $2 -g 960x720 --plugin cliprdr --ignore-certificate $3 }`

Ezután pedig úgy kapcsolódok különböző szerverekhez hogy `rdpw Felhasznalo jelszo ide.kapcsolod.ok` és már megy is minden.

(igen tudom hogy lassan kéne csinálnom egy külön blogot a tech dolgoknak)
