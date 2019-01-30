---
author: KTamas
categories:
  - Export
date: 2009-03-11 20:00:35
guid: http://ktamas.blog.hu/2009/03/11/a_mi_eseteink
id: 1769345
disqus_identifier: 1769345
url: /index.php/2009/03/11/a_mi_eseteink/
permalink: /index.php/2009/03/11/a_mi_eseteink/
tags: [szerverek, windows]
title: A mi ESETeink
---

<span style="font-size: 20px">一</span> Furcsa hibát kap az egyik kolléga: definíció-frissítés után random program tökéletes exe fájlját véli vírusosnak a _Nod_. Ezek után rövid úton szétfagy a gép, vagyis megszűnik reagálni mindenre a reset gombon kívül. Újraindítás után szinte azonnal ugyanez, gép szétterhelődik, egy start menü fél óra mire megjelenik. 

Hopp, mégegy gép. 

Hopp, mégegy&#8230; óbazdmeg. Felmegyünk a _Nod_ fórumjára, hamar kiderül, nem mi vagyunk az egyetlenek a problémával. Mindeközben több gép használhatatlan, és mivel a kedves _Nod_ service természetesen széf módba is elindul&#8230; aztán nagy nehezen sikerül elég gyorsan eljutni a gépeken Serviceshez és letiltani a kis rohadékot, majd átnevezni a Nod32 mappáját, hogy esélye se lehessen elindulni. Mindeközben körbejárni az összes gépet és letiltani az automatikus frissítést illetve a ThreatSense.NET-et (mert ennek is köze volt a dologhoz), hogy legalább ott ne legyen katasztrófa. Pár óra múlva jön a frissítés ami orvosolja a problémát. 

<span style="font-size: 20px">二</span> A fájlszerver eltűnik a hálózatról. Ja, meg a többi is. Beüt a &#8220;Szétfagyott a Szerver Valamiért&#8221; Rendszergazdai Gyomorgörcs &#8482;. A szerver épp újraindul a kékhalálból&#8230; ami különösen ciki, hogy ez a főszerver volt, ami fut jópár virtuális szerver, ja, és ezt ugye kb. 30 ember használta épp. A _Nod_ restart után nem működik, a megoldás az ESET oldala szerint egyszerű: uninstall, restart, programmappa töröl, reinstall, restart. Hát persze. A fórumokon csak egy-két hasonló eset másoktól, úgyhogy reménykedés hogy ez csak valami izo&#8212;- 

Hová tűnt a fájlszerver? Remote desktop indít, hopp, de szép kék halál a fájlszerveren (ez &#8216;csak&#8217; egy virtuális gép). Restart után ezen se megy a _Nod_, ismeretlen hiba. 

Elmegyek ebédelni, mire visszaérek, a Lock Computer helyén a Press CTRL+ALT+DEL to log in virít. 

Mindhárom gép 64-bites volt, így hajlanék arra, hogy csak ezeket érinti, ámde! Kolléga gépe még reggel, a szerverlefagyás előtt, szintén kifagyott, és egy gyors dumpanalízis azt mutatta, hogy azt is a _Nod_ csinálta. Mindenesetre a maradék gépek az irodában zakatoltak tovább. Következő este pedig vírusirtó-újratelepítés lett&#8230; 

<span style="font-size: 20px">三</span> Kora reggel. Még csak egy páran vagyunk bent az irodában, egy, már szabadságon lévő kolléga rámszól Skype-on, hogy a _Nod_ szerint több rendszerfájlja vírusos. WTF? Mondja, hogy azért majd még körülnéz, mert valami nem stimmel neki se ebben. Itt benn mindenki gépe rendben. 

Már később olvasom <a href="http://www.neowin.net/forum/index.php?showtopic=744544" target="_blank">ezt az apró hírt</a>: az új definíció felrakása után rendszerfájlokat írthat a _Nod_&#8230; 

**Epilógus** 

Lehet, hogy régimódi vagyok, de vannak bizonyos elvárásaim a biztonsági szoftverekkel szemben. Ezek közé bizony beletartozik az, hogy ne gyilkolásszon rendszereket, meg taszítsa őket kék halálba&#8230; egyelőre azért marad, mert a többi vírusirtóról is megvan a véleményem, mindenesetre mostmár a Nod32-ben sem bízok. A <a href="http://i.gizmodo.com/5083371/a-call-for-revolution-against-beta-culture" target="_blank">beta culture</a> pedig kapja be. 

(A HVG-s címért én kérek elnézést)
