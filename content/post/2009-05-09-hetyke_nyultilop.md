---
author: KTamas
categories:
  - Export
date: 2009-05-09 10:30:35
guid: http://ktamas.blog.hu/2009/05/09/hetyke_nyultilop
id: 1769381
disqus_identifier: 1769381
url: /index.php/2009/05/09/hetyke_nyultilop/
permalink: /index.php/2009/05/09/hetyke_nyultilop/
tags: [linux, ubuntu, windows]
title: Hetyke Nyúltilop
---

Szóval eljött az április, és eljött az Ubuntu 9.04 is, a próba kedvéért felraktam mind az asztali (munkahelyi) gépemre, mind a laptopomra. Az eredmények, nos, vegyesek. 

Asztali gép: wifi nincs, viszont van videókártya (hehe), mégpedig ATi, abból is egy X300. A rendszer telepítés után nem hajlandó bekapcsolni a Compizt, a restricted drivers nem mutat semmit. Felrakom manuálisan a bináris drivert, halál, vesa módba kell kapcsolnom az X-et hogy újra életre keljen. Fél óra nyomozás után ellentmondásos információkat kapok, a legigéretesebbnek az tűnik, hogy ez a driver már nem támogatja az X300-at, csak azt nem sikerül megtudni, hogy akkor mi is. Itt jegyezném meg, hogy nem tudom, komolyan gondolták-e, hogy alapból kikapcsolva van a Ctrl+Alt+Backspace billkombó, de viccnek durva. 

Mindenesetre, fájdalmasan lemondva a Compizról, egy meglepően használható és gyors rendszert kapunk. A Gnomeon a legutóbbi verzió óta políroztak egyet, berakták az új notification rendszert, hármas openoffisz (az UI ikonjai határozottan rondák továbbra is), és sok egyéb apróságot. Belekerült a rendszerbe a screen-profiles is, ami a screen használatát könnyíti meg mindenféle előre elkészített scripttel (amit utána szabadon módosíthatunk). 

Körülbelül egy hétig használhattam a rendszert, és meglepően megkedveltem. Sajnos azt a problémát továbbra se oldja meg, hogy bizonyos, a munkámhoz elengedhetetlen programok továbbra is csak windowson futnak (hello, Trados!), úgyhogy sajnos 1-2 naponta kellett valamiért elővenni valamelyik virtuális gépet a szerveren. Viszont, mikor egész nap pl. linux szervereket izélgettem, egyáltalán nem hiányzott a windows (és a putty). Még a narancsárga alaptémát is megszoktam pár nap alatt, sajnos a linuxos Skype mondjuk butus, a Pidgin pedig továbbra is néha minden szó nélkül elszáll. Viszont a Gnome Do továbbra is a nambervan segédprogram. De izé, szóval az egész rendszer határozottan jó irányba indult el, csak ne rontsák el a Gnome 3-mat. 

Sajnos ekkor ütött be egy váratlan alaplapprobléma, úgyhogy kénytelen voltam 1-2 napig a laptopomat használni, amiben viszont van wifi (oh boy&#8230;) és Intel videokártya (jáááááááááj). Meglepő módon a wifivel nem nagyon volt gond &#8212; igaz kell neki reboot után úgy egy perc mire kapcsolódik, de ha az megvan, akkor megy &#8211;, a videokártya, na az viszont. [Írtam már](http://ktamas.blog.hu/2009/01/26/a_wind_es_az_ubuntu_esete_pt_1) korábban a problémáról, de a legnagyobb egyelőre az, hogy laaaaaaaassssú. 2D-ben is. Két ablak között a váltás 1-2 másodperc, ami egyszerűen nevetséges. Lehet downgradelni Intrepides driverekre, midnenféle módokkal kisérletezni (EXA, UXA, XAA, ABC, BFG, CBA etc.) de sehogy se tudtam emberi sebességre hozni, arról nem is beszélve h anno a compiz amúgyis érdekes glitcheket produkált. Úgyhogy fájdalmas búcsút vettünk egymástól, és rebootoltam vissza Windows 7-be. 

Mindenesetre, ha helyreáll az asztali gép, nem kizárt, hogy tovább fogom használni, már amikor tudom, mert hosszútávon nincs értelme annak, ha az egyetlen nyitott ablak egy terminal services client valamelyik virtgépünkre&#8230;
