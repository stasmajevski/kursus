# Eesrakenduste arendamine 2017k

* **Kursuseprogramm:** [IFI6211](#)
* **Õpetaja:** Romil Rõbtšenkov, [romilr@tlu.ee](mailto:romilr@tlu.ee)
* **Testserver:** lin2.tlu.ee, greeny.cs.tlu.ee
* **Tunni näited:** [~romil/ea17k](http://minitorn.cs.tlu.ee/~romil/ea2017k)

### Ühendus Greeny'sse

* Windows | [VIDEO](https://youtu.be/kg5NAsRQAJ8)

    * [Guide to create tunnel (in estonian, but with screenshots)](http://minitorn.tlu.ee/~jaagup/kool/java/kursused/09/veebipr/naited/greenytunnel/greenytunnel.pdf)

* Mac OS | [VIDEO](https://youtu.be/RJc-Gvpn9M4)
```
1. open Terminal app

2. write:
ssh university_username@lin2.tlu.ee -L 5555:greeny.cs.tlu.ee:80
3. then write TLU password

    Now you can access greeny from browser localhost:5555

3. open new tab in Terminal (cmd+t) and write:
ssh university_username@lin2.tlu.ee -L 2222:greeny.cs.tlu.ee:22
4. then write TLU password

5. now open FTP client (CyberDuck, FileZilla, Coda) for example and connect to greeny via SFTP
    host: localhost or some require 127.0.0.1 (127.0.0.1 = localhost)
    port: 2222
    username: your_greeny_username
    password: your_greeny_username

6. choose one Terminal tab and connect to greeny via ssh, write:
ssh greeny_username@greeny.cs.tlu.ee
7. then enter your Greeny username password
    ls             – to view files and folders in current path
    cd folder_name - to enter folder
    cd ..          – to exit folder to previous path

```

## Kodused tööd ja projektid

* [1. kodutöö](https://github.com/eesrakenduste-arendamine-2017k/1.ea-kodutoo)
* 2. kodutöö
* 3. kodutöö
* [projekt](https://github.com/eesrakenduste-arendamine-2017k/ea-projekt-2017k)

**Kodused tööd peavad olema lõplikult valmis eksamiajaks. Pikendust pärast eksamiaega paranduste tegemiseks ei saa!**

### GitHub'i töövoog

1. *Fork*'i ülesande/projekti repositoorium (leiab [https://github.com/eesrakenduste-arendamine-2017k/](https://github.com/eesrakenduste-arendamine-2017k/)).
1. *Clone*'i see repositoorium enda arvutisse/serverisse ja määra repositooriumi URL kuhu edaspidi muudatusi salvestad.
  ```
  git clone https://USERNAME@github.com/USERNAME/REPOSITORY.git
  ```
1. Lisa ka oma nimi ja email repositooriumi omanikuks ([Setting your username](https://help.github.com/articles/setting-your-username-in-git/))
1. Muuda faile ülesande lahendamiseks ja *Commit*'i iga olulisem muudatus, kasutades kahte käsku.
  ```
  git add .
  ```
  ```
  git commit -m "Added this functionality to the app"
  ```
1. Veendu, et kogu kood on *Commit*'itud.
  ```
  git status
  ```
1. *Push/sync*'i GitHub'i.
  ```
  git push origin
  ```
1. [Ava *pull request*](https://help.github.com/articles/creating-a-pull-request) ülesande originaalses repositooriumis. Ülesannete tähtajaks on 24h enne järgmise tunni algust, kui pole teisiti kirjas.
1. Muudatusi ja täiendusi võib *push*'ida repositooriumisse, kuni ette antud  kuupäevani.

Tagasisidet saab otse *pull request*'i millele ootan Sinupoolseid kommentaare/mõtteid/küsimusi. Võid julgselt avada *pull request*'i kohe kui hakkad kodutöö kallal tegelama ja siis kui hätta jääd võid esitada sinna küsimuse. Maini kommentaaris minu kasutajat `@romilrobtsenkov` siis jõuan sellele kiiremini vastata.

### Nõuded

Need rakenduvad ka päris elus!

* Peab järgma "head programmeerimise stiili"
    * Muutujate nimed peavad kirjeldama muutujat ning peavad olema inglise keeles
    * Funktsiooni nimi peab olema "lühike"
    * Optimeeri koodi lugemiseks
    * Projektide jaoks tuleb kasutada objektorienteeritud lähenemist
    * Laenatud koodile tuleb viidata
* Boonuspunktid:
    * Loomingulisus (NB! nõuded peavad olema täidetud)

## Kursus
### 1. tund

1. Sissejuhatus
    * Veebiprogrammeerimise aine kokkuvõte
    * Arutleme, mis antud kursus endas hõlmab
1. Ajalugu
    * ECMAScript
    * iframe > XMLHttpRequest > AJAX
1. JS kasutusvaldkonnad
    * Lehtede interaktiivseks muutmine ([awwwards](http://www.awwwards.com), [cssdesignawards](http://www.cssdesignawards.com))
    * Võrgu koormuse vähendamine
    * AJAX
    * Vormide valideerimine
    * WebSocket ([Chat](http://socket.io/get-started/chat/))
    * Mängud ja meelelahutus ([threeJS](https://threejs.org))
    * Brauserite lisateegid
1. JS piirangud
    * Andmete kirjutamine serverisse
    * Ligipääs andmebaasidele
    * Ligipääs failisüsteemile
    * Akende sulgemine
    * Lõimtöötlus
    * Ligipääs teistele veebilehtedele
    * Browserite erinevused
1. Turvalisus
   * JS koodile ligipääs
   * `window.opener` näide ([On the security implications of window.opener.location.replace()](https://blog.whatever.io/2015/03/07/on-the-security-implications-of-window-opener-location-replace/) by julio)
1. Tunnis kasutatavad tööriistad
1. Javascript'is programmeerimine, näidisrakenduse loomine
    * muutujad, funktsioonid, aeg, sündmuste kuulamine, dokumendi muutmine
1. [1. kodutöö](https://github.com/eesrakenduste-arendamine-2017k/1.ea-kodutoo)
1. **Kohustuslik järgmiseks korrasks!**
   * **Vaata kuidas ja mis järjekorras JS ning brauser koostööd teevad [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ) by Philip Roberts**
   * **Singleton muster [Learning JavaScript Design Patterns](https://addyosmani.com/resources/essentialjsdesignpatterns/book/) by Addy Osmani**

### 2. tund

1. JS rakenduse ülesehitus (objektorienteeritud kood)
    * JS "use strict" – [w3schools](http://www.w3schools.com/js/js_strict.asp), [ECMAScript 5 Strict Mode](http://ejohn.org/blog/ecmascript-5-strict-mode-json-and-more/)
    * *single-page-application* artikli põhjal [Reimagining Single-Page Applications With Progressive Enhancement](https://www.smashingmagazine.com/2015/12/reimagining-single-page-applications-progressive-enhancement/)
    * Kasutame Singleton mustrit (Loe kindlasti mustrite kohta lähemalt [Learning JavaScript Design Patterns](https://addyosmani.com/resources/essentialjsdesignpatterns/book/) by Addy Osmani)

### Praktikum 
[1. kodutöö](https://github.com/eesrakenduste-arendamine-2017k/1.ea-kodutoo) lõpetamine + küsimused

## Materjalid ja tööriistad

### Tunnis kasutatud rakendused
* [Atom](https://atom.io), lisad emmet, jshint(aegunud), linter, linter-jshint, atom-beautify
* koodi valideerimine [JSLint](http://jslint.com) / [JSHint](http://jshint.com)
* debug:
    * [Chrome Developer Tools](https://developer.chrome.com/devtools/index)
        * [Official debugging tutorial](https://developer.chrome.com/extensions/tut_debugging)
        * õpetus [JavaScript Diagnosis](http://www.macwright.org/2015/03/10/javascript-diagnosis.html)
    * [Firefox Developer Edition](https://www.mozilla.org/en-US/firefox/developer/)

### Kohustuslik materjal

Välja toodud tundide loetelu juures vastavalt igale tunnile.

### Soovituslik lugemine

* [Kliendipoolsed veebirakendused](http://www.tlu.ee/~jaagup/skriptkeeled/kliendirakendused.pdf)
* [Google JavaScript Style Guide](https://google.github.io/styleguide/javascriptguide.xml)
* [JavaScript Garden](http://bonsaiden.github.com/JavaScript-Garden/)
* [Mozilla's Introduction to Object-Oriented Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript)
* [Mozilla Developer Network](https://developer.mozilla.org/en/JavaScript)
* [Learn JavaScript](https://developer.mozilla.org/en-US/learn/javascript)
* [w3schools](http://www.w3schools.com/jsref/default.asp)
* [What’s so great about JavaScript Promises?](http://blog.parse.com/learn/engineering/whats-so-great-about-javascript-promises/)
* [Front-end Job Interview Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions)
* [JavaScript Best Practices](http://www.thinkful.com/learn/javascript-best-practices-1/)
* [JavaScript Patterns](http://shichuan.github.io/javascript-patterns/)
* [Learning Advanced JavaScript slides](http://ejohn.org/apps/learn/)
* [Static Web Apps](http://www.staticapps.org/)
* [The JavaScript Interpreter, Interpreted](http://www.slideshare.net/marthakelly/js-interpreter-interpreted) [(video)](https://www.youtube.com/watch?v=iSxNCYcPAFk)
* [Classical Inheritance in JavaScript](http://www.crockford.com/javascript/inheritance.html)
* [Partial Application in JavaScript](http://benalman.com/news/2012/09/partial-application-in-javascript/)
* [Learning JavaScript Design Patterns](http://addyosmani.com/resources/essentialjsdesignpatterns/book/)
* [JS: The Right Way](http://www.jstherightway.org/)
* [Code School](https://www.codeschool.com/paths/javascript)
* [Javascript Trail Map](https://upcase.com/javascript)
* [How To Learn JavaScript Properly](http://javascriptissexy.com/how-to-learn-javascript-properly/)
* [Superhero.js](http://superherojs.com)
* [Teach Yourself to Code](http://teachyourselftocode.com/javascript)

### PHP meeldetuletus
* [PHP Coding Style Guide](http://www.php-fig.org/psr/psr-2/)
* [Veebirakenduste loomine PHP ja MySQLi abil](http://minitorn.tlu.ee/~jaagup/kool/java/loeng/veebipr/veebipr1.pdf)
* [PHP with MySQL Essential Training](http://www.lynda.com/MySQL-tutorials/PHP-MySQL-Essential-Training/119003-2.html)

#### HTML/CSS/JS sandbox'id

* [JS Bin](http://jsbin.com/)
* [CodePen](http://codepen.io/pen/)
* [JSFiddle](http://jsfiddle.net/)

### Git
* [Become a git guru.](https://www.atlassian.com/git/tutorials/)

## Litsents
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />Käesolev <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" rel="dct:type">leht</span> ja kõik teised https://github.com/veebiprogrammeerimine-2015s materjalid on <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International Litsensiga</a>.
