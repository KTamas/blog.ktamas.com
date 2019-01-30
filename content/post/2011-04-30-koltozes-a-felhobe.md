---
author: KTamas
categories:
  - Uncategorized
date: 2011-04-30 18:17:56
fb-status-updater-meta:
  - a:5:{s:22:"custom-facebook-status";s:0:"";s:21:"custom-twitter-status";s:0:"";s:7:"fb-push";s:1:"1";s:7:"tw-push";s:1:"1";s:4:"push";s:1:"1";}
fb-status-updater-sn-reference:
  - a:2:{i:0;a:2:{i:0;s:8:"facebook";i:1;s:27:"722715145_10150170515360146";}i:1;a:2:{i:0;s:7:"twitter";i:1;s:17:"64393066534019072";}}
guid: http://blog.ktamas.com/?p=2362437
id: 2362437
disqus_identifier: 2362437
url: /index.php/2011/04/30/koltozes-a-felhobe/
permalink: /index.php/2011/04/30/koltozes-a-felhobe/
tags: [énblog, linux, meta, programozás, szerverek]
title: Koltozes a felhobe
---

Ket dolog tortent, az egyik, hogy mostanaban folyton elszallt a php-nginx kombo egyszercsak [a 64 megas VPS-en](http://blog.ktamas.com/index.php/2010/10/12/64-megabytes-should-be-enough-for-everyone/), amit anno osszeraktam. Frissitettem, megneztem a konfigokat, megis, egyszercsak elhalt az egesz, kezzel kellett ujrarugni. A masik dolog, ami tortent, hogy mikor tegnap este ismetelten kaptam a pingdomtol emailt, hogy &#8220;DOWN alert: blog (blog.ktamas.com) is DOWN&#8221;, akkor azt mondtam, hogy oke, eljatszotta az utolso lehetoseget is a helyzet, holnap (azaz ma) uj VPS-t keresunk. 

Azaz, kerestunk volna, mert ma reggel kaptam egy emailt, ami igy kezdodott:

> &#8220;You have been selected to enter the PHP Fog Beta program!&#8221;

A masik dolog, ugyanis ami mostanaban tortent, az az volt, hogy egyre-masra bukkannak fel a [hacker news](http://news.ycombinator.com/)on [Heroku](http://www.heroku.com/)-szeru cloudos PaaS-ok (Platform as a Service), eloszor talan pythonhoz-djangohoz, majd kesobb mindenfele mas programnyelv/framework/egyeb kombohoz. Mint anno a betas Heroku, ok is altalaban ingyenes betakra epulnek, hogy az emberek jol kibetatesztelik az ingyenes/olcso szolgaltatasert cserebe az egeszet. Raadasul a deployment szinte kivetel nelkul giten keresztul megy, ami iszonyat kenyelmesse teszi a dolgot, mostanaban egyre tobb projekten dolgozok amihez amugyis azt hasznalom ([itt a githubom](http://www.github.com/ktamas/), nem disznolab). De eloreszaladok, ez egy masik blogposzt temaja lesz, remelhetoleg hamarosan.

Szoval kaptam PHP Fog betat, amire miert is ne alapon bejelentkeztem meg circa szuk ket honapja, megcsinaltam az accountot, csinaltam egy uj wordpress appot (fel evig ingyenes a legkisebb csomagban, aztan majd meglatjuk), kidumpoltam az adatbazist a regi szerveren, kimasoltam a gepemre a regi wordpress mappammal egyutt, git-cloneoztam a repot arrol az URL-rol, amit a PHP Fog adott nekem, felulirtam a wp-content mappat a regivel, behuztam PhpMyAdminbol a regi adatbazist, eeees&#8230; futottam meg egy kort a supporttal, mert hiaba pusholtam a szerverre, hiaba mondta h sikeres, a friss wordpress telepites nem nagyon latta a repoba rakott fajlokat. Mindenesetre dicseretes, hogy a szupportosok szombat ellenere par ora alatt valaszoltak es megjavitottak a helyzetet, atraktam a domain A-rekordjat, ujraimportaltam a DB-t mert azota irtam egy posztot, es most meg eppen ezt irom.

A felho tehat borzasztoan kenyelmesse tesz dolgokat, ami persze nem jelenti azt, a helyzet felhotlen lenne (elnezest), az elmult napokban is voltak erre peldak, ugye, mindenesetre programozooldalrol tenyleg iszonyat kenyelmesse tesz dolgokat, hogy (kis tulzassal) git push, es szevasztok. A bennem levo controlfreak rendszergazda most epp el van tehat nyomva, de biztos ki fog jonni egyszercsak&#8230;
