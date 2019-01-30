---
author: KTamas
categories:
  - Uncategorized
date: 2011-07-05 16:17:07
fb-status-updater-meta:
  - a:5:{s:22:"custom-facebook-status";s:0:"";s:21:"custom-twitter-status";s:0:"";s:7:"fb-push";s:1:"1";s:7:"tw-push";s:1:"1";s:4:"push";s:1:"1";}
fb-status-updater-sn-reference:
  - a:2:{i:0;a:2:{i:0;s:8:"facebook";i:1;s:27:"722715145_10150230503395146";}i:1;a:2:{i:0;s:7:"twitter";i:1;s:17:"88250076685803520";}}
guid: http://blog.ktamas.com/?p=2362595
id: 2362595
disqus_identifier: 2362595
url: /index.php/2011/07/05/huawei-e1752-meg-az-osx/
permalink: /index.php/2011/07/05/huawei-e1752-meg-az-osx/
tags: [agymenes, mac]
title: Huawei E1752 meg az OSX
---

Szolíd linuxos élményben volt részem a Huawei E1752-es számú mobilnetjével a Macbookon, ugyanis megszűnt működni egyszercsak. Először azt hittem, egy korábbi Time Machine-os restore kavart be, de utólag kiderült, szűz rendszeren se megy jól a driver, igaz máshogy törik. Mindenesetre egy firmware frissítés csináltam a modemen (az nem segített), majd rábukkantam valamelik Telenor oldalon (Dán? Norvég? one of those.) a gány Mobile Connect.app nélküli drivercsomagra, ami egyébként [innen letölthető](http://www.huaweidevice.com/resource/mini/200910149695/testmobile1014/index.html). Először persze le kellett irtani mlg az írmagját is a régi drivernek, ebben segítségemre volt a rootban kiadott `'find . -iname '*huawei*'` és az ezekre kiadott `rm -rf `kombója, minden kext-app-plist-modemscript törlése után működött az új driverrel a már [ismert módon](http://blog.evandavey.com/2008/02/how-to-connect-huawei-e220-usb-modem.html), akár a [cheetahwatch](http://thepatrick.com.au/cheetahwatch/)csal is.

(Tanulság, az nincs, maximum, hogy a mobilnet nyomokban még mindig szopás tud lenni.)
