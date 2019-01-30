---
author: KTamas
categories:
  - Uncategorized
date: 2011-05-05 23:58:46
fb-status-updater-meta:
  - a:5:{s:22:"custom-facebook-status";s:0:"";s:21:"custom-twitter-status";s:0:"";s:7:"fb-push";s:1:"1";s:7:"tw-push";s:1:"1";s:4:"push";s:1:"1";}
fb-status-updater-sn-reference:
  - a:2:{i:0;a:2:{i:0;s:8:"facebook";i:1;s:27:"722715145_10150174809575146";}i:1;a:2:{i:0;s:7:"twitter";i:1;s:17:"66260584542388224";}}
guid: http://blog.ktamas.com/?p=2362476
id: 2362476
disqus_identifier: 2362476
url: /index.php/2011/05/05/iframek-es-popupok-toredekek-a-fejleszto-naplojabol/
permalink: /index.php/2011/05/05/iframek-es-popupok-toredekek-a-fejleszto-naplojabol/
tags: [javascript, programozás, random]
title: iframek es popupok (toredekek a fejleszto naplojabol)
---

Van egy iframed, abbol nyit a felhasznalo egy popupot, kulso webszolgaltatassal valo autenikalas celjabol, adsz neki egy callback URL-t, ami viszont ugye a popupba iranyit vissza, te viszont szeretned, ha az iframe tartalma lecserelodjon, majd bezarodjon a popup. Hogy csinalod? Ugy, hogy egy ilyesfajta HTML-t (es benne levo js-t) adsz meg callbacknek:


<noscript>
  </p> 
  
  <pre>
&lt;html&gt;
  &lt;head&gt;
    &lt;script type="text/javascript"&gt;
      var close_and_redirect = function() {
        if (opener && !opener.closed) {
          opener.location.href = "http://localhost:9610/done";
        }  
        window.close();
      }
    &lt;/script&gt;
  &lt;/head&gt;
  &lt;body onload="setTimeout('close_and_redirect()', 500)"&gt;
    Yay, logged in! Closing...
  &lt;/body&gt;
&lt;/html&gt;
</pre>
  
  <p>
    </noscript><br />
  </p>
  
  <script src="https://gist.github.com/958052.js?file=loggedin.html"></script>
  
  <p>
    (<a href="http://www.codingforums.com/showpost.php?s=aa079e493200cb7008aa5359f7591e86&#038;p=292432&#038;postcount=3">Itt talaltam meg vegul.</a>)
  </p>
