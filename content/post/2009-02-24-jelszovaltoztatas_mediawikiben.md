---
author: KTamas
categories:
  - Export
date: 2009-02-24 13:06:09
guid: http://ktamas.blog.hu/2009/02/24/jelszovaltoztatas_mediawikiben
id: 1769333
url: /index.php/2009/02/24/jelszovaltoztatas_mediawikiben/
permalink: /index.php/2009/02/24/jelszovaltoztatas_mediawikiben/
tags: [wtf]
title: Jelszóváltoztatás Mediawikiben
---

Napi találós kérdés: hogyan változtatjuk meg egy adott user jelszavát Mediawiki alatt ha adminok vagyunk? _Természetesen_ így:

> ### <a href="http://meta.wikimedia.org/wiki/MediaWiki_FAQ#How_do_I_change_a_user.27s_password.3F" target="_blank"><span class="mw-headline">How do I change a user&#8217;s password?</span></a>
> 
> Assuming that <var>$wgPasswordSalt</var> is set to true (the default), you can use the following SQL query:
> 
> <pre>UPDATE user SET user_password = MD5(CONCAT(user_id, '-',<br />
  MD5('somepass'))) WHERE user_name = 'someuser';</pre>

Ha jön a forradalom, mennek a falhoz.
