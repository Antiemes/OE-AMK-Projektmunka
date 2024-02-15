# Numerikus billentyűzettel vezérelhető akadályelkerülő játék

A játék háromdimenziós, ahol a játékos egy repülővel, vagy
űrhajóval halad előre. Vele folyamatosan akadályok kerülnek
szembe. Az akadályok egy 3x3-as rácson foglalhatnak helyet
és magának a játéknak az irányítása is egy 3x3-as rács logikájára
épül. A numerikus billentyűzeten helyet foglaló számok megnyomásakor
a repülő / űrhajó az adott számnak megfelelő pozícióban folytatja útját.

Példa:

A numerikus billentyűzet elrendezése:

| 7 | 8 | 9 |
|---|---|---|
|**4**|**5**|**6**|
|**1**|**2**|**3**|

Tegyük fel, hogy középen vagyunk és így haladunk előre.
Ekkor középen előbukkan egy akadály. Áthúzódunk balra
(4-es gomb), így elkerüljük az akadályt. Majd egy újabb akadály
jön jobbra fent (biztonságban vagyunk), majd bal oldalt.
Ezt kikerülendő átlépünk mondjuk a bal felső helyre (7-es gomb).

Fontos követelmény, hogy az akadályoknak (természetesen) véletlenszerűen
kell érkezniük és nem lehet egyszerre az összes mezőben akadály.

