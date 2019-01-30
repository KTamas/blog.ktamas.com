---
author: KTamas
categories:
  - Uncategorized
date: 2013-08-09 11:01:47
guid: http://blog.ktamas.com/?p=2365144
id: 2365144
disqus_identifier: 2365144
url: /index.php/2013/08/09/kozerdeku-kozlemeny-service-order-avagy-a-halozati-kapcsolatok-prioritasa/
permalink: /index.php/2013/08/09/kozerdeku-kozlemeny-service-order-avagy-a-halozati-kapcsolatok-prioritasa/
tags: [osx, random, windows]
title: 'Közérdekű közlemény: Service Order, avagy a hálózati kapcsolatok prioritása'
---

Mivel most szívom meg többedszerre ezzel, leírom, hátha segít valaki másnak is. Szóval, adott az a helyzet, amikor az embernek egynél több hálózati kapcsolata aktív: egyszerre van fent céges hálózaton wifivel meg kábellel, esetleg bekapcsolva hagyta az ájfónján a Personal Hotspotot és bedugta szinkronizálni, vagy éppen 3G/4G-ről internetezik, és felkapcsolódik a céges VPN-re. 

Oké, de ilyenkor mi kap prioritást? Az, ami feljebb van a listán. Milyen listán?

Windows 7 alatt is, meg OSX alatt is jól el van rejtve ez. Az előbbi alatt az [itt található leírást](http://windows.microsoft.com/en-us/windows7/change-the-order-of-network-protocol-bindings) kell követni a megfelelő ablak eléréséig, míg OSX alatt a System Preferences &#8211; Network &#8211; fogaskerék ikon baloldalt lent &#8211; Set Service order&#8230; menüpont alatt lehet beállítani a megfelelő sorrendet. Ezzel elkerülhető az, amibe például legutóbb futottam, hogy a céges VPN-re kapcsolódva 3G/4G-ről hirtelen elment az internetem, mert magasabb volt a prioritása a kapcsolatnak, míg wifin ez nem jött elő, mert azt még régebben a megfelelő helyre ráncigáltam az említett listán&#8230;
