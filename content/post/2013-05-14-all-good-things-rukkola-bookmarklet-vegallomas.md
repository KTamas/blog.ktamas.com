---
author: KTamas
categories:
  - Uncategorized
date: 2013-05-14 08:55:13
guid: http://blog.ktamas.com/?p=2364599
id: 2364599
disqus_identifier: 2364599
url: /index.php/2013/05/14/all-good-things-rukkola-bookmarklet-vegallomas/
permalink: /index.php/2013/05/14/all-good-things-rukkola-bookmarklet-vegallomas/
tags: [rukkola]
title: All good things (Rukkola bookmarklet, végállomás)
---

**Nagyon rövid verzió:** mostmár minden oldalon (a kiemelt könyvek között is, a profiloldalon is) megy a happoló mód, így nyugdíjaztam a bookmarkletet.

Az úgy volt, hogy tavaly megszületett a rukkola, én pedig nagyon lelkesen indultam neki az oldalnak, mint felhasználó. Aztán elkezdett zavarni az, hogy nem lehet szűrni a csak happolható könyvekre, úgyhogy [írtam rá egy bookmarkletet](http://blog.ktamas.com/index.php/2012/08/11/hacking-rukkola-avagy-alternativ-kollekciobongeszes/).

Az idők során aztán [került bele végtelen görgetés](http://blog.ktamas.com/index.php/2012/08/15/rukkola-bookmarklet-update-1-gorgetes-a-vegtelenbe/), [kapott egy saját oldalt](http://blog.ktamas.com/index.php/rukkola-bookmarklet/), tanultam egy csomó dolgot, például azt, hogy nem szabad az ilyesmit a GitHubon tartani, szóval [költözött is egyet](http://blog.ktamas.com/index.php/2012/08/16/rukkola-bookmarklet-update-2-growing-pains/), majd mikor már meg voltam elégedve a funkcionalitással, [újraírtam az egészet](http://blog.ktamas.com/index.php/2012/09/15/rukkola-bookmarklet-update-3-%E3%83%AA%E3%83%A9%E3%82%A4%E3%83%88/), hogy a kód is kinézzen valahogy. Mindenközben tanultam egy csomó dolgot, amit [megosztottam az egyik javascript meetupon](http://blog.ktamas.com/index.php/2012/10/16/my-adventures-in-the-world-of-bookmarklets-meg-mindig-benne-vagyok-az-internetben-rovat/).

Aztán hogy, hogynem, egyrészt [a funkcionalitás egy jórésze bekerült magába a rukkolába](http://blog.ktamas.com/index.php/2012/10/18/rukkola-bookmarklet-update-4-this-is-not-a-goodbye/), ezzel elérve a célját, másrészt pedig külsősből belsős lettem: és elkezdtem a rukkolánál rendszergazda lenni, jelentősen felgyorsítani az oldal bizonyos részeit, bugokat javítani, meg közben robotokat vadászni. 

A bookmarklet azért továbbra is használatban volt, sőt, pár hónapja reneszánszát élte, amióta felfedezték az emberek, hogy a kiemelt könyvek oldalon nem működik a beépített happoló mód, ellenben a bookmarklet igen. Én közben kiköltöztem Svédországba, azóta a bugfixelgetésben nem vagyok már benne, csak néha nézek fel a szerverre, kirugdosni egy-egy újabb robotot, meg úgy általában a háttérben lévő, csendes rendszergazdaként működök aki néha helyrerúgja a szervert, ha nem viselkedik rendesen.

A bookmarklet most pedig végleg befejezte a pályafutását: mostmár minden oldalon működik a happoló mód, a kiemelt könyvek között is. Így most kiélesítettem az új verziót, ami csupán egy üzenet arról, hogy már nincs szükség az egészre. Ami, mint azt sokszor elmondtam, mindig is a végcél volt.

Szemfüles olvasóknak és felhasználóknak feltűnhet, hogy ezzel eltűnt a végtelen görgetés is: egyrészt az a funkciót sosem csináltam meg úgy igazán rendesen, másrészt sajnos se motivációm, se időm nincs a dologra. Valamint úgy látom, remekül megvan az oldal nélküle is. Arról nem is beszélve, hogy a jelenlegi implementációja bizonyos helyzetekben feleslegesen terheli a szervert. 

Ha azonban valaki késztetést érez a dologra, hogy mégis megcsinálja: a bookmarklet kódja eddig is és továbbra is nyílt forráskódú, [megtalálható a GitHubon](https://github.com/KTamas/rukkola_hacks).

És aztán az is lehet, hogy egyszercsak rámjön az ötperc, és mégis megcsinálom, de ezt megigérni egyelőre nem tudom. Mindenesetre köszönet minden felhasználónak és minden visszajelzésnek.
