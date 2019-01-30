---
author: KTamas
categories:
  - Export
date: 2010-03-09 10:30:00
guid: http://ktamas.blog.hu/2010/03/09/when_in_doubt_run_process_monitor
id: 1823449
disqus_identifier: 1823449
url: /index.php/2010/03/09/when_in_doubt_run_process_monitor/
permalink: /index.php/2010/03/09/when_in_doubt_run_process_monitor/
tags: [random, windows]
title: When in doubt, run Process Monitor
---

> [&ldquo;When in doubt, run Process Monitor!&rdquo; (I follow this advice religiously, even having my daughter run Process Monitor when she comes to me with a homework question)](http://blogs.technet.com/markrussinovich/archive/2010/01/13/3305263.aspx)

Felvésem ide is, mert örök értékű szabály ez. Tegnap az SQL Express 2008 SP1 telepítője dobott furcsa hibákat, amire a [megadott Microsoft KB](http://support.microsoft.com/kb/300956/en-us) adott mégfurcsább és méghomályosabb nemválaszokat. [Kis guglizás után](http://www.symantec.com/connect/articles/install-and-configure-sql-server-2008-express#comment-2751821) pedig&#8211; a [Process Explorer](http://technet.microsoft.com/en-us/sysinternals/bb896653.aspx)en keresztül &#8212; eljutottunk a [Process Monitor](http://technet.microsoft.com/en-us/sysinternals/bb896645.aspx)ig, ami megmondta, melik registry bejegyzést kell hova klónozni, hogy működjön a telepítés.

&nbsp;
