---
author: KTamas
categories:
  - Export
date: 2010-03-25 20:00:00
guid: http://ktamas.blog.hu/2010/03/25/blackberry_bold_es_az_os5
id: 1867923
disqus_identifier: 1867923
url: /index.php/2010/03/25/blackberry_bold_es_az_os5/
permalink: /index.php/2010/03/25/blackberry_bold_es_az_os5/
tags: [ajánló, blackberry, szeder]
title: Blackberry Bold (9000) és az OS5
---

Már egy jó ideje <strike>szivárogtatja a RIM</strike> szivárognak ki az újabbnál újabb OS5 buildeket mindenféle Berryhez, köztük az én 9000-emhez is, sőt, egy-egy szolgáltató már hivatalos verziókat is kiad, így egyszercsak meguntam a várakozást, hogy majd fél év múlva megjön a magyar T-hez (jó esetben), utánaolvastam a [megfelelő](http://forums.crackberry.com/f3/how-wipe-jl_cmder-53502/) [threadekben](http://forums.crackberry.com/f83/newest-official-os-5-0-0-509-blackberry-bold-9000-wind-hellas-431443/) a crackberryn, letöltöttem a legújabb Desktop Managert, és a frissítést, és nekiláttam a mellékelt instrukciók szerint, ami egyébként a következő:

  1. **Kijelentkezünk mindenből** a Berryn, különösen a Google Syncből és a Facebookból.
  2. Letöltöd az új DM-et és frissítést [innét](https://www.blackberry.com/Downloads/entry.do?code=3210DDBEAA16948A702B6049B8D9A202). Ha a rendszer személyes adatokat kérdez tőled, élsz állampolgári jogaiddal, és megadod neki Steve Jobsot és az 1 Infinite Loopot. El fogja fogadni.
  3. Miután mindkettőt feltelepítetted, a&nbsp;c:\Program Files\Common Files\Research In Motion\AppLoader\ mappából törlöd a vendor.xml fájlt. Esetleg átnevezed, a lényeg, hogy ne legyen ott.
  4. Letöltöd és felrakod a JL_Cmder nevű segédeszközt [innét](http://forums.crackberry.com/f3/how-wipe-jl_cmder-53502/). Feldugod a gépre a Szedret, backupot készítesz a Desktop Managerrel, biztos helyre elrakod három példányban.
  5. Elindítod a JL_Cmdert, kiválasztod a 4-es opciót (wipe), végigköveted az utasításokat. Ez letakarít **minden** adatot a szederről, és körülbelül fél percet vesz igénybe
  6. Ezen a ponton a Bold kijelzője töksötét, csak a piros LED világít. Elindítod az AppLoadert (c:\Program Files\Common Files\Research In Motion\AppLoader\Loader.exe), nyomogatod a Next-eket, ha minden jól megy, eljutsz arra a kijelzőre, ahol kiválaszthatod, mit akarsz még felrakni a szederre, az alaprendszeren kívül. Érdemes tényleg csak azt felrakni, amire szükség van, jótékony hatással van a rendszerre és az elérhető memóriára.
  7. A Wizard végén a Finish gombra kattintva elindul a frissítés, amely négy lépésből áll. Az elsőben felrakja az alaprendszert, ennél nem kell problémának lennie. Ezután újraindul a Berry, majd egy szép fehér képernyőre jut, ekkor kell(ene) detektálnia újra az AppLoadernek, hogy folytassa a hármas és négyes ponttal, az alkalmazások felrakásával. Ha sokáig próbálkozik felismerni, de a végén, csak egy hibát dob, hogy nem találja (Retry/Cancel), akkor nem esünk pánikba, hanem lehúzzuk a Szedret, majd pár másodperc után feldugjuk, várunk egy kicsit majd nyomunk neki egy Retryt, ekkor azonnal fel kell ismernie, és végigcsinálnia a procedúrát, aminek a végén megintcsak újraindul.
  8. Ezután úgy 5 percig egy Blackberry feliratú képernyő tölt, a végén meg már az ismert elsőindításos képernyő fogad, amin gyorsan végig lehet menni.
  9. Hurrá, van OS5 a Szedrünkön!

Ezen a ponton el lehet kezdeni újratelepítgetni mindenféle thirdparty programot, majd miután ezzel megvagyunk, elindítjuk a Desktop Managert, a Backup and Restore -> Advanced ponton betöltjük (File > Open)&nbsp;a hármas pontban elkíszített backupunkat, és **csak a szükséges adatbázisokat** visszatöltjük (az én esetemben ez nem is volt sok, csa az Address Book, a Phone History és az SMS-ek, meg esetleg az e-mailek). A full restore nem ajánlott, netes fórumokon legalábbis sok problémát ahhoz társítanak.

**So what&#8217;s new?**

Szebb rendszer, threaded SMS support, sokkal gyorsabb böngésző, sok-sok egyébb apróság, egyelőre még felfedezés alatt van, meg fogom írni, amiket találok. Egyéb random gondolatok:

  * Google Talkot desktopról kell telepíteni, mert valamiért az m.google.com/talk-nak nem tetszik az ötös böngésző.
  * A Keyboard Lock úgy tűnhet, hogy eltűnt, valójában azonban átalakult: ha beállítunk jelszót, akkor visszakapjuk a 4.x-os módot, ikonnal-mindennel, ha nem, akkor a * (A) gomb kb. 1 másodpercig való nyomásával lehet lezárni a billentyűzetet, illetve az egész rendszert standbyba rakni. Ebből a Mute gombbal lehet felébreszteni.
  * T-n a böngésző neve Web&#8217;n&#8217;Walk&#8230;
  * A rendszer **sokkal** gyorsabban indul újra: kb. egy perc a megszokott 4-5 helyett
  * Okosabb Bedside Mode! (lásd 1. kép)

Első ránézésre tehát szép és jó az új rendszer, akksiidőről, stabilitásról, ilyesmiről több tapasztat szerzése után írok majd.&nbsp;   
**   
(Disclaimer: mindenki saját felelősségére frissít, ha valahol valami elromlik, azért felelősséget nem vállalok etc.)**

![](http://ktamas.blog.hu/media/image/BBScreenShot_3.png)

![](http://ktamas.blog.hu/media/image/BBScreenShot.png)
