Avagy "okos ember más hibáiból tanul" - rovat. Vannak olyan hibák, amiket a legtöbb kezdő fordító elkövet, ezekből álljon itt egy kis gyűjtemény.

Hamis barátok
=============

{ ! angol !! magyar !! megjegyzés |- | virtually || ~~virtuálisan~~ <ins>gyakorlatilag</ins> || |- | specific || ~~speciális~~ <ins>különleges, egyedi</ins> || |- | powerful || ~~erőteljes~~ <ins>hatékony</ins> || |- | technically || ~~technikailag~~ <ins>szigorúan véve</ins> || |- | tricky || ~~trükkös~~ <ins>nehéz, problémás</ins> || |}

"A %s-hez..."
=============

A %s és úgy általában, minden változó névelője "a(z)". Két-vagy háromalakú toldalékot pedig nem kap, ugyanezért: mert akármi állhat helyette, nem tudhatjuk, melyik kell. Az egyalakú toldalékok (-ig, -kor, stb) elfogadhatók. A ragozás megkerülésére használt módszerek:

-   ha tudjuk, hogy micsoda a %s (fájl, könyvtár, plazmavető): "a(z) %s \[ fájlhoz | könyvtárhoz | plazmavetőhöz \]"
-   ha nem tudjuk, vagy több dolog is lehet: "a következőhöz: %s"
-   ha kis helyre kell beszorítani, vagy egy beviteli mező előtt áll egy "to:" (vagy hasonló): "ehhez:"

"<programneve> is a ..."
========================

Az angol eredetiben gyakran láthatóak ehhez hasonló szerkezetek, névjegy panelen vagy állapotjelzésként, magyarul viszont elég rosszul néz ki az, hogy "Gaim egy multifunkciós csevejkliens". Nyugodtan tegyünk elé egy névelőt, sokkal értelmesebb / jobban néz ki az, hogy "A Gaim egy multifunkciós csevejkliens".

"\_Ignore"
==========

"K\_ihagy"

Kihagyás, hasonlóan a kivágás, másolás, mentés, megnyitás, stb-hez (de: "alkalmaz", a szabály erősítése és a gombok szélességével való spórolás témája miatt) hasonlóan.

"Mondatközi Nagybetűk"
======================

Általános hiba, hogy ha egy mondaton belül több szó is nagybetűvel kezdődik, azt a magyarban is nagybetűvel kezdik. Ez helytelen, a magyar helyesírás ugyanis nem ismer ilyet (ez Nem a Német Nyelv :) ) és a [GNOME HIG](http://library.gnome.org/devel/hig-book/stable/design-text-labels.html.en#layout-capitalization) sem vonatkozik rá.

Gyorsbillenty\_ű ékezet előtt
=============================

Lehetőleg ne használjuk. Nem feltételezhetjük ugyanis, hogy mindenki, aki magyar nyelven akarja a grafikus felületű alkalmazásokat használni, rendelkezik magyar billentyűzettel/magyar kiosztást használ.

Gyorsbillentyűk ütközése
========================

Ha egy menün/ablakon belül több menüpont/vezérlőelem is ugyanazzal a gyorsbillentyűvel rendelkezik, akkor annak megnyomása sorrendben aktiválja a vezérlőelemeket, amelyeket a szóközzel/enterrel lehet ténylegesen kiválasztani. Ez megnehezíti a program használatát, így kerülendő. Elkerülésére több, együttesen használandó módszer kínálkozik: - A fordítási fájlban egymást követő sztringek figyelése. Ezek jó eséllyel azonos ablakhoz/menühöz tartoznak, így az ezek közötti átfedések megszüntetése javasolt. - A magyar nyelvben ritkábban előforduló betűk használata, például: c, d, o, p, u, z - Végül az elkészült fordítás tesztelése a program verziókövetőben lévő verziójával.

Két szóköz mondatvégi pont után
===============================

Az angol eredetiben van, magyarul: nincs.

Szóköz sztringek végén
======================

Az előbbihez hasonló jelenség amikor sztring végén is áll egy szóköz, például:

` msgid "Options "`
` msgstr "Beállítások "`

Ezt a szóközt általában azért érdemes meghagyni, mert a kedves programozó sietett és nem állított be [normális térközt](http://library.gnome.org/devel/hig-book/stable/design-text-labels.html.en#layout-label-position), helyette egy szóközzel javított a felület megjelenésén. Praktikus hibaként bejelenteni és kérni az eredetiből a szóköz eltávolítását, akár hivatkozva az imént linkelt Gnome HIG-re (ha az adott projektnél ezt figyelembe veszik).

Két sztringből álló mondatok
============================

Néha előfordul, hogy egy mondat két külön msgid-ben van leírva, a kettő között pedig általában valamilyen felületi elem például léptetőgomb áll. Ezt arról lehet felismerni, hogy egymás után két fél-mondat áll, amik "mintha" összetartoznának, és a megjegyzésben az előfordulási helyük csak néhány (&lt;10) sornyira van egymástól. Ilyenkor nem kell nagyon ragaszkodni külön-külön az eredeti sztringek értelméhez, elég, ha a két üzenet együtt adja vissza a teljes mondat értelmét. Például:

` msgid "S_witch off after:"`
` msgstr "Kika_pcsolás:"`

` msgid "minutes"`
` msgstr "perc után"`

Ez a programban valahogy így néz ki: Kika\_pcsolás: &lt;10&gt; perc után

Nem elérhető, nem kikereshető, nem feldolgozható, nem visszaváltható
====================================================================

Gyakran látni ezekhez hasonló helytelen szerkezeteket kezdő fordítók munkáiban, és egyéb helyeken is, de ezeket ettől még nem érhető el, nem kereshető ki, nem dolgozható fel (és: nem váltható vissza) alakban kell helyesen írni.

6:3
===

A rövidítés azt jelenti, hogy a három vagy több szóból és hat vagy több szótagból (egy szótagú igekötők és toldalékok nélkül) álló szóösszetételeket a fő összetételi határon kötőjellel kapcsoljuk össze, az olvashatóság megkönnyítése érdekében.

A kétszavas összetételeket egybeírjuk. Például: menüikon, szintaxiskiemelés, sortörés. Az eredetiben ezek általában külön állnak, de ez ne tévesszen meg.

Speciális helyeken lévő üzenetek
================================

Gyakran fordulnak elő olyan üzenetek, amelyek többféleképpen értelmezhetők/fordíthatók, attól függően, hogy hol vannak a programban, például ugyanaz a szöveg lehet egy parancssori kapcsoló, egy program vagy (GNOME esetén) egy GConf-kulcs leírása ugyanúgy, mint egy, a felhasználótól adatokat bekérő ablak címsora, így kezdő fordítók néha az előbbi három esetén is megszólítják a felhasználót, ami adott esetben szükségtelen. Ezeket arról lehet felismerni, hogy a főprogram első &lt;1000 sorában vannak (ez általában a programneve --help segítségével ellenőrizhető), vagy .desktop.in illetve .schemas.in fájlokban. ([FIXME](FIXME "wikilink"): hasonlók még?)

Például, a "Specify a value" üzenet "Érték megadása"-ként fordítandó, ha a fenti három feltétel egyike teljesül, illetve "Adjon meg egy értéket"-ként, ha nem.

CSUPANAGYBETŰS szavak
=====================

Általában ezek a parancssori kapcsolók paramétereit jelölik, például: --prefix PREFIX. Parancssori kapcsolók esetén maga a kapcsoló nem fordítandó, a csupa nagybetűs szó viszont igen.

GConf-kulcsok és -értékek
=========================

Ez egy GNOME-specifikus dolog, a GConf konfigurációs adatbázisban gyakran fordul elő, hogy a kulcsok leírásai más kulcsok nevére hivatkoznak, illetve ha a kulcs értéke néhány sztring típusú elem egyike kell legyen, akkor ezeket leírással együtt felsorolják. .schemas.in fájlokban fordulnak elő, a szabály velük kapcsolatban az, hogy a kulcsneveket és -értékeket nem fordítjuk (a GConf ezt nem támogatja) és a lehetséges értékek mögé zárójelben odatesszük a fordítást, ha van értelme, például: "Az ablak elhelyezkedése. Lehetséges értékek: top (fent), bottom (lent)". (Nyilván ha n darab kódlapból kell egyet választani, akkor nem.)

Mondatvégi írásjelek
====================

Általában, ha az eredetiben nincs, akkor a fordításban sincs. Felszólító mondatok után, hacsak nem hangsúlyozott felszólításról/figyelmeztetésről van szó, nincs felkiáltójel! Például: "Válasszon ki egy dokumentumot" (fájlválasztó ablak címsora).

A szöveg érthetősége mindenek felett
====================================

Az alábbi rész a [Fordítás HOGYAN](http://tldp.fsf.hu/Forditas-HOGYAN/Forditas-HOGYAN.html) oldalról származik, mondandóját érdemes megszívlelni:

-   A munka megkezdése előtt nézd át a szógyűjteményt, amely egyes angol szavak magyar megfelelőjét tartalmazza a [MLDP](MLDP "wikilink") szerint.
-   Nézz bele egy-két magyarított HOGYANba, és az egyes részeket hasonlítsd össze azok angol változatával. Így könnyebben ráérzel arra, mit és hogyan kell és/vagy érdemes fordítanod.
-   Ragaszkodj az angol eredeti szöveg értelméhez, mondanivalójához, de ne ragaszkodj annak megfogalmazásához/mondatszerkezetéhez.
-   Angolul teljesen másképp kell gondolkodni, mint magyarul. Előfordulhat, hogy egy angol mondatot két magyar mondatra érdemes fordítani és viszont.
-   A minőségi munka érdekében inkább lassan, de precízen fordíts. Teljesen felesleges összedobni valami ferdítés félét, aztán a lektorra bízni, hadd fordítsa le újra az egészet...
-   Ha valamely szó, kifejezés vagy mondat jelentésében bizonytalan vagy illetve végképp nem boldogulsz, kérdezz rá a levelezőlistán, amelyre a [A Magyar Linux Dokumentációs Projekt](https://lists.sch.bme.hu/wws/info/linuxhowto) honlapon iratkozhatsz fel. A lista ugyanis ezért (is) van.
-   Ha az angol szó vagy kifejezés látszólag nem illik a mondatba, akkor gyanakodj! Valószínűleg többértelmű szóról/kifejezésről van szó. Például a "double check" kifejezést többen, csont nélkül "dupla ellenőrzés"-nek fordították, ez annyira magyartalan, hogy csak na. A "double check" helyesen "alapos ellenőrzés". Ilyen esetben használjátok a fordítási segédleteket, ha végképp nem boldogulsz, akkor a teendőket lásd az előző bekezdésben.
-   A munka végeztével olvasd végig fordításodat a helyesírási hibákat is figyelve/javítva. Ha épeszű magyar emberként megérted amit abban leírtál, valószínűleg jó munkát végeztél. Tartsd észben: a fordításokat a Linux-felhasználók népes tábora olvassa.

