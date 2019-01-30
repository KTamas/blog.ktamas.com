---
author: KTamas
categories:
  - Uncategorized
date: 2012-01-30 10:20:52
fb-status-updater-meta:
  - a:5:{s:22:"custom-facebook-status";s:0:"";s:21:"custom-twitter-status";s:0:"";s:7:"fb-push";s:1:"1";s:7:"tw-push";s:1:"1";s:4:"push";s:1:"1";}
fb-status-updater-sn-reference:
  - a:2:{i:0;a:2:{i:0;s:8:"facebook";i:1;s:27:"722715145_10150500254430146";}i:1;a:2:{i:0;s:7:"twitter";i:1;s:18:"163914573462765568";}}
guid: http://blog.ktamas.com/?p=2362992
id: 2362992
url: /index.php/2012/01/30/sharewood-hu-kontentmegosztas-harmadik-resz/
permalink: /index.php/2012/01/30/sharewood-hu-kontentmegosztas-harmadik-resz/
title: Sharewood.hu (kontentmegosztás, harmadik rész)
---

> &#8230;Ha összerakunk [a megosztásokhoz] egy, a különböző feedek elemeit összesítő és megjelenítő [planetet](http://en.wikipedia.org/wiki/Planet_(software)), akkor beljebb leszünk kicsit.

&#8230;[írta Kelt](http://worldshots.hu/2012-01/csinaltam-egy-linkblogot/) még a [múltkor](http://blog.ktamas.com/index.php/2012/01/23/kontentmegosztas-redux-tamadnak-a-linkblogok-come-and-join-the-revolution/). Közben eltelt egy hét és már tizen vagyunk, szóval lassan, de biztosan nő a közösség. Én pedig pár napja nekifogtam a dolognak, és mostanra került olyan állapotba, hogy vállalható legyen, szóval minden további időhúzás nélkül, kattintsatok: [sharewood.hu](http://sharewood.hu/)

Az oldal olvasása mellett fel lehet iratkozni annak az [RSS](http://feeds.feedburner.com/Sharewoodhu)-ére, ha valaki mindenki megosztását egy helyről szeretné olvasni, vagy letölthet egy [OPML](http://sharewood.hu/sharewood_opml.xml)-t amit aztán kedvenc RSS-olvasójába importálhat és kiválogatja, kiket szeretne olvasni.

És ami a legfontosabb, ha csatlakozni akarsz hozzánk, [írj nekünk egy ímélt](mailto:join@sharewood.hu), és hozzáadunk. Ha hibát találsz az oldalban, vagy ötleted van, vagy akármi, [akkor is írj nekünk](mailto:info@sharewood.hu).

A dolog technikai részletei:

Kezdtem az [eredeti Planet](http://planetplanet.org) szoftverrel, macera volt, kényelmetlen, de azt mondtam oké, ha megy, akkor legyen, elkezdtem összerakni a dolgot. Nagyjából akkor hajítottam ki az ablakon, mikor a képekkel kezdődő posztokat szimplán elrontotta.

Ekkor találtam rá a [Venus nevű forkjára](http://intertwingly.net/code/venus/), ami egy fokkal kevésbé volt bugos, és miután a [levelezőlistán elmondták](http://lists.planetplanet.org/archives/devel/2012-January/002248.html), hogy hol tudom kiszedni azt a fícsört, hogy az iframes embedeket kitépi a posztokból, már majdnem boldog voltam, de. A venus (és a planet is) szimplán legenerál egy statikus lapot az utolsó x elemből, és ennyi, se archívum, se több oldalra tördelés, se keresés, se semmi, szóval ezt kicsit kevésnek éreztem.

A végén a planetrubyonrails.([com](http://planetrubyonrails.com)|[net](http://planetrubyonrails.net)) [motorjánál](https://github.com/anildigital/planet) kötöttem ki. Ezt jól [megforkoltam](https://github.com/KTamas/sharewood.hu), felfrissítettem a legfrissebb Railsre, átírtam benne jópár dolgot és összebaltáztam egy dizájnt, aminek egyik felét [Kelt Világlövésétől](http://worldshots.hu/), a másikat [Dave Winer Scripting Newsától](http://scripting.com) loptam. Ha van önként jelentkező egy jobb dizájnra, azt szivesen fogadjuk.

Szóval így állt össze a [Sharewood](http://sharewood.hu) mostani állapota.

&nbsp;
