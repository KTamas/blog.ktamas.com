---
author: KTamas
categories:
  - Export
date: 2009-01-10 13:16:01
guid: http://ktamas.blog.hu/2009/01/10/sargetol_a_hyper_v_ig_masodik_resz
id: 1769305
url: /index.php/2009/01/10/sargetol_a_hyper_v_ig_masodik_resz/
permalink: /index.php/2009/01/10/sargetol_a_hyper_v_ig_masodik_resz/
tags: [linux, szerverek]
title: Sargetól a Hyper-V-ig, második rész
---

Szóval ott tartottunk a sztorival hogy naív kislányként úgy gondoltam, hogy akkor majd berakom RAID-be utólag (háháháhá). Mint az kiderült, ez nem annyira egyszerű, főleg ha LVM is van az adott winchin, amit én &#8220;miért is ne&#8221; alapon raktam fel &#8212; igen, ekkor még elég kezdő linuxos voltam. Mindenesetre nagy nehezen sikerült levadásznom egy laza 8 oldalas guideot a howtoforge-ról, és nekiestem, gondoltam megvan pár óra alatt (háháháhá). Ez gyakorlatilag egy éjszakányi szívást jelentett&#8230; ugyanis, pár nappal azelőzőleg backupként át-dd-ztem (igen, tudom, hülyeség) egy másik winchire az adott winchit backup okán, na most ez azt eredményezte, hogy teljesen meghülyült az mdadm (ez a linuxos softraid progi), mert a két winchit teljesen megegyezőnek látta. Mindenesetre reggelre sikerült megcsinálni úgy, hogy működjön igaz újraindítani már nem tudtam a dolgot, mert gondok voltak a /etc/fstab-bal&#8230; ezt egy újabb pár órányi szívás helyretette. 

Volt még pár elég furcsa linuxos szívásom, például mikor a rendszer úgy döntött ő most fél napnyi adatot korruptál, azóta se tudni miért, és azt se, miért csak az aznapi adatok&#8230; 

Majd folytatjuk.
