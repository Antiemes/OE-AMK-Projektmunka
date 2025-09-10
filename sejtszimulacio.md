# Sejtszimuláció hatszögrácson

A projekt célja egy hatszögrács alapú sejtszimuláció elkészítése grafikus szemléltetéssel.
A szimulációban kétféle növény és kétféle gomba vesz részt. Minden cellában ezek közül
egy lehet (emellett lehet a cella üres is). Minden cella meghatározott mennyiségű
vizet és kétféle anyagot is tárol. Az egyik anyag az egyik típusú növényt serkenti a növekedésben,
a másik a másikat, a másik növényt viszont mindkét anyag elpusztítja. Mindkét növény
akkor tud növekedni, ha a saját cellájában, vagy körülötte megfelelő mennyiségű víz
és tápanyag van. Ha a "serkentő" gomba által termelt anyag is jelen van, akkor
gyorsabban. Növekedéskor ezeket az anyagokat értelemszerűen elhasználja a növény.
Ha elfogy a tápanyag, akkor nem tud tovább terjeszkedni, de nem pusztul el. Ha
elfogy a víz, akkor a növény elpusztul. A gomba terjeszkedéséhez csak víz
és magának a gombának a jelenléte kell; a gomba egy bizonyos idő után automatikusan elpusztul.
Az élőlények elpusztulásakor a felhasznált tápanyag és víz visszakerül azokba a
cellákba, ahol az élőlény addig volt.

A szimuláció egyes paramétereinek beállítása (például hogy pontosan milyen gyorsan terjeszkednek
az egyes növények és gombák) a csapat feladata. Ezt célszerű úgy beállítani, hogy egyik
élőlény se tudja teljes egészében kiszorítani a másikat.

## A program elvárt funkciói

  * Kezdőállapot előállítása (tápanyag és víz gócok, kiinduló élőlény telepek).
  * Anyagok és élőlények kézi elhelyezése.
  * Szimuláció lépésenként történő futtatása.
  * Szimuláció adott sebességű folyamatos futtatása.
  * Statisztikai adatok rögzítése (élőlény telepek mérete stb.).
  * Állapot mentése és visszatöltése.

## Egyéb teendők a projekthez

  * Tesztek futtatása.
  * Paraméterek hangolása.

