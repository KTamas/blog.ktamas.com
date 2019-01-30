---
author: KTamas
categories:
  - Export
date: 2009-11-15 23:33:54
guid: http://ktamas.blog.hu/2009/11/15/huje_postgresql
id: 1769464
disqus_identifier: 1769464
url: /index.php/2009/11/15/huje_postgresql/
permalink: /index.php/2009/11/15/huje_postgresql/
tags: [linux, random, szerverek]
title: Hüje PostgreSQL
---

Akkor most random rendszergazdai puffogás következik, muszáj leírni. 

Szóval az történt hogy kedvenc céges projektkezelonket migráltam 7.4-es Postgresrol 8.1-re, pontosabban új szerverre, de ezzel járt eme váltás is.  Minden rendben ment &#8212; kivéve, hogy a timesheet feature (ki mit hol mennyit dolgozott) hirtelen megszunt muködni, ahol ugye napokhoz vannak rendelve projektek és idok. Nézegettem a program kódját, semmi, SVN-bol checkoultoltam, de minden stimmelt, áthoztam a régi szerverrol a program mappáját, hátha mégiscsak változott valami, de nem. Újraimportáltam az adatbázist, hátha valami hiba elkerülte a figyelmem, de nem, minden rendben. Akkor kezdjünk el querykkel játszani mindkét szerveren&#8230; hoppá. 

Ami a régi szerveren 2009-01-10 00:00:00+01 az az újon 2009-01-09 23:00:00+00&#8230; igen, minden ido szépen GMT-hez lett igazítva, így minden egy napot ugrott vissza, pontosabban az elozo napra ugrott vissza. Túrtam a netet, és a konfig fájlokat, de semmit se találtam. Így [megkérdeztem lazywebet (olvasd: megkérdeztem a ServerFaulton)](http://serverfault.com/questions/84927/postgresql-7-4-8-1-migration-timezone-issue), és meg is lett a megoldás: az új verzióval kell a régi szervert dumpolni! 

Nem baj, úgyis hajat akartam vágni, csak most kicsit furcsák a kopasz foltok a fejemen&#8230;
