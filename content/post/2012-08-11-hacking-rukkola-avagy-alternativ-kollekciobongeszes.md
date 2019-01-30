---
author: KTamas
categories:
  - Uncategorized
date: 2012-08-11 18:31:15
fb-status-updater-meta:
  - a:5:{s:22:"custom-facebook-status";s:0:"";s:21:"custom-twitter-status";s:0:"";s:7:"fb-push";s:1:"1";s:7:"tw-push";s:1:"1";s:4:"push";s:0:"";}
guid: http://blog.ktamas.com/?p=2363197
id: 2363197
url: /index.php/2012/08/11/hacking-rukkola-avagy-alternativ-kollekciobongeszes/
permalink: /index.php/2012/08/11/hacking-rukkola-avagy-alternativ-kollekciobongeszes/
tags: [programozás, rukkola]
title: Hacking Rukkola, avagy bookmarklet a nem happolhatóak elrejtésére
---

Szóval elindult a [rukkola.hu](http://rukkola.hu/), közösségi könyvcserélde, remek dolog, próbáljátok ki, felteszitek a megunt könyveiteket, és cserébe szerezhettek másoktól hasonlókat. A böngészés a feltett könyvek között egyelőre még nem tökéletes, engem például borzasztóan zavar, hogy a [kollekciók](http://rukkola.hu/kollekciok) böngészésénél (szerk: és keresésnél) nincs olyan nézet, amikor csak azokat a könyveket látom, amikre ténylegesen lecsaphatok.

Összedobtam hát gyorsan egy bookmarkletet erre. Chrome Extensionnek indult, de nem érzem elég nagynak, hogy megérje berakni a saját App Storejukba, valamint sóher vagyok kifizetni az öt dollárt érte egyelőre, majd ha még lesz pár ilyen rukkola-módosításom, amit már érdemes felrakni. Mindenesetre nincs más dolgoktok, hogy [felrakjátok a bookmarklet oldaláról](http://blog.ktamas.com/index.php/rukkola-bookmarklet/). <del datetime="2012-08-15T16:30:01+00:00">Lapozni a Tovább gombbal lehet, még az oldalakat is mutatja.</del> **Update:** nem kell semmit kattintgatni, [van végtelen görgetés](http://blog.ktamas.com/index.php/2012/08/15/rukkola-bookmarklet-update-1-gorgetes-a-vegtelenbe/).

**Update 2:** A bookmarklet frissült és saját oldalt kapott, [innen rakhatod fel](http://blog.ktamas.com/index.php/rukkola-bookmarklet/).

A mostani megoldásnak megvan az a hátránya, hogy ha átkattintasz egy könyvre, akkor sajnos kezdheted elölről. Ez egy 0.0.<del datetime="2012-08-15T16:30:01+00:00">1</del>2-es változat, a 0.0.<del>2</del>3-ben majd ezt is áthidaljuk valahogy remélhetőleg és/vagy egyszer a távoli jövőben ha lesz Rukkola API, majd arra fogunk építkezni.

A teljes kód [fent van a githubon](https://github.com/KTamas/rukkola_hacks/tree/bookmarklet) természetesen. <del datetime="2012-08-15T16:40:33+00:00">Könnyen megoldható lenne, hogy az összes oldalt betöltse egyszerre, de ezt nem szeretném, mert feleslegesen terhelném vele a rukkola szervereit, amik amúgyis elég lassúak tudnak lenni sajnos sokszor. Esetleg a jövőben valamiféle végtelenscrollozást belerakok, és akkor a Továbbra kattintgatást megússza az ember.</del> [Van végtelen görgetés!](http://blog.ktamas.com/index.php/2012/08/15/rukkola-bookmarklet-update-1-gorgetes-a-vegtelenbe/)

És egy before-after kép, avagy előtte:

[<img src="/wp-content/uploads/2012/08/rbefore-439x1024.jpg" alt="" title="Előtte" width="439" height="1024" class="aligncenter size-large wp-image-2363219" srcset="/wp-content/uploads/2012/08/rbefore-439x1024.jpg 439w, /wp-content/uploads/2012/08/rbefore-128x300.jpg 128w, /wp-content/uploads/2012/08/rbefore.jpg 1009w" sizes="(max-width: 439px) 100vw, 439px" />](/wp-content/uploads/2012/08/rbefore.jpg)

És utána:

[<img src="/wp-content/uploads/2012/08/rafter-400x1024.jpg" alt="" title="Utána" width="400" height="1024" class="aligncenter size-large wp-image-2363218" srcset="/wp-content/uploads/2012/08/rafter-400x1024.jpg 400w, /wp-content/uploads/2012/08/rafter-117x300.jpg 117w" sizes="(max-width: 400px) 100vw, 400px" />](/wp-content/uploads/2012/08/rafter.jpg)

(P.S.: RSS-ből valószínű biztosan nem fog működni a bookmarkletes dolog, szóval ha ezt a Google Readerben olvasod, át kell hozzá kattintani)

(P.P.S.: A bookmarklet remekül alkalmazható keresésekre is.)