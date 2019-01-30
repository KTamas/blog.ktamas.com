---
author: KTamas
categories:
  - Export
date: 2009-01-08 11:34:49
guid: http://ktamas.blog.hu/2009/01/08/sargetol_a_hyper_v_ig_elso_resz
id: 1769304
disqus_identifier: 1769304
url: /index.php/2009/01/08/sargetol_a_hyper_v_ig_elso_resz/
permalink: /index.php/2009/01/08/sargetol_a_hyper_v_ig_elso_resz/
tags: [linux, szerverek]
title: Sargetól a Hyper-V-ig, első rész
---

Szóval az egész úgy kezdődött hogy elkezdtem dolgozni, és pár hónap után már mint társrendszergazdaként (is) tengettem az életem. Az akkori felállás egyszerű volt: 1 db szerver, rajta egy (már akkor kicsit outdated) Debian Sarge, Samba a fájloknak meg egy Apache a projektkezelőrendszernek. A hálózatos háttérről is fogok írni majd de az egy másik post lesz. 

Szóval így kezdtünk, sajnos szegény szerver egy kis kondi nélküli szobában tengette az életét, amit bizony megsínylett, talán emiatt lehetett az, hogy az alaplap IDE, majd később a SATA vezérlője is erősen hisztis volt, és egy idő után egyre több nagyon gyanús hibát dobált. 

Szóval akkor alaplapcsere. Én akkor még elég kezdő voltam linuxban, de hallottam hogy az még az alaplapcserét is túléli (háháháhá). Winchi átrak, power gomb megnyom, kernel pánik. <a href="http://mentalstatic.info/blogs/" target="_blank">Linuxos ismerős</a> zaklatása, hát bizony a Sarge kernele nem nagyon ismeri a vadiúj alaplap ICH9R-jét. Backportsból új kernel, de nem elég új&#8230; akkor új Linux. Ubuntu Gutsy Server fel, aztán meg mindenféle dolgok konfigurálása Dutow (lásd Linuxos ismerős) aktív zaklatása mellett. A végére mindenesetre megtanultam egy rakat dolgot. Persze LVM-mel installáltam (virtuális partíciómanager), és gondoltam majd utólag berakom RAID-be (háháháhá). 

Tu bí kontinjúd&#8230;
