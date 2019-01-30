---
author: KTamas
categories:
  - Export
date: 2009-05-24 12:16:24
guid: http://ktamas.blog.hu/2009/05/24/imap_is_a_ghetto
id: 1769389
url: /index.php/2009/05/24/imap_is_a_ghetto/
permalink: /index.php/2009/05/24/imap_is_a_ghetto/
tags: [imap, linux, mail]
title: IMAP is a ghetto
---

Az van, hogy van ez az IMAP, ami jó. Szerveren tárolhatsz mindent, megosztott mappák, satöbbi, olyan, mint az Exchange, csak jobb. Lenne. Viszont. 

一 Az Outlook egy fos, mint aztmár egy [előző blogpostomban](http://ktamas.blog.hu/2009/05/17/die_outlook_die) is fejtegettem. Sok shared mappa esetén a Send & Receive kb. egy percig tart, ami idő alatt az Outlook még mai gépeken is majd&#8217; használhatatlanul lassú lesz. Ezenfelül egy aranyos, kb. 6 éve ismert bug miatt ha az ember leiratkozik olyan mappákról, amiben olvasatlan levelek vannak, akkor az outlook figyelmen kívül hagyva minden beállítást, azonnal kiküld egy rakat &#8220;Not Read:&#8221; értesítést minden üzenetre, amire read receipt lett kérve. 

二 Így lett nekünk az új céges levelezőkliens a Thunderbird: ez gyors, nem küld ki kéretlenül leveleket leiratkozáskor, cserébe a Subscribe funkció egyelőre erősen bugzik benne (random felirat mappákra, illetve nem irat le róluk), és nem tudok rájönni, hogy miért. Debug módban konkrétan egy rakat ilyen hibát kapok:

> 1628149872[1e71f20]: considering playing queued url:imap://user@my.mail.server.address:143/unsubscribe>.shared/a/sub/folder 
> 
> -1628149872[1e71f20]: creating protocol instance to play queued url:imap://user@my.mail.server.address:143/unsubscribe>.shared/a/sub/folder 
> 
> -1628149872[1e71f20]: failed creating protocol instance to play queued url:imap://user@my.mail.server.address:143/unsubscribe>.shared/a/sub/folder

三 Webmailnek a legjobb perpillanat a Roundcube, ami viszont szeret néha teljesen értelmetlen &#8220;error: undefined&#8221; hibákat adni, kicsit még éretlen (0.4-es verzió&#8230;), valamint szintén szocproblémái vannak a feliratkozással, konkrétan ha az erre szolgáló oldalra megyünk a beállításokban, akkor 10-ből 9-szer felirat azonnal az összes mappára, szintén nem tudom, hogy miért.. 

Gyanakszom, hogy esetleg valami szerveroldali hiba, de már háromszor végignéztem a Courier beállításait, és sehol se láttam semmit ami bekavarhatna&#8230;
