---
author: KTamas
categories:
  - Uncategorized
date: 2012-05-01 23:11:01
fb-status-updater-meta:
  - a:5:{s:22:"custom-facebook-status";s:0:"";s:21:"custom-twitter-status";s:0:"";s:7:"fb-push";s:0:"";s:7:"tw-push";s:0:"";s:4:"push";s:1:"1";}
guid: http://blog.ktamas.com/?p=2363116
id: 2363116
disqus_identifier: 2363116
url: /index.php/2012/05/01/nagy-fajlok-feltoltese-wordpressre-rakjukel/
permalink: /index.php/2012/05/01/nagy-fajlok-feltoltese-wordpressre-rakjukel/
title: Nagy fájlok feltöltése wordpressre (rakjukel)
---

PHP-CGI és Nginx kombóban az alábbi értékeket kell módosítani, igen, mindhármat:

a `php.ini`ben:
  
`upload_max_filesize = 64M<br />
post_max_size = 64M`

az `nginx.conf`ban, a server blokkon belül:
  
`client_max_body_size 64M;`

Restart mindkettő (lehet elég reload is) és máris tudunk nagyobb tartalmakat feltölteni.
