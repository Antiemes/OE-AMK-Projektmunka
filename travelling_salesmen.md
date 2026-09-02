# Utazó úgynök stratégiai játék

Az utazó ügynök egy jól ismert NP-teljes probléma, ahol a cél röviden az, hogy
előre meghatározott célokat (az eredeti megfogalmazásban városokat) tetszőleges
sorrendben, de minimális összes úton bejárjunk. Ez a projekt e köré épít egy
hálózati többjátékos (pseudo) körökre osztott stratégiai játákot.

A játék rács alapú. Egy rácspont lehet üres, de lehet rajta meglátogatandó célpont,
vagy valamilyen akadály, ahova a játékos nem tud lépni, illetve felvehető "powerup".
A pályákat egy szöveges pályafájlból kell beolvasni (a fájlban minden karakter
egy mezőnek felel meg).

A játékosok egy megadott startmezőről indulnak és körönként egyet léphetnek valamelyik
szomszédos mezőre (átlós lépés nem megengedett). Ez normál esetben szigorúan felváltva,
vagy kettőnél több játékos esetén egy bizonyos sorrendben haladva történne. Azonban
megengedjük, hogy a játékosok néhány (de nem sok) lépéssel előrébb, vagy hátrább
járhassanak egymáshoz képest, így a körökre osztottság nem teszi darabossá a játékmenetet.

A játékosok felvehetnek "powerupokat" is, amikkel előnyt szerezhetnek (például két
lépés egy körben), vagy a többi játékost hátrányhoz juttathatják (akadály
elhelyezése a pályán). Az akadály lehet egy teli mező, amire egyáltalán nem
lehet lépni, vagy egy, a mező határvonalán elhelyezett fal. Ezeket a játékos
a saját mezője szélén helyezheti el. Az akadály elhelyezése is egy lépésnek számít.

A játék többjátékos rendszerű, ahol mindenki a saját karakterét irányítja,
de látja a többi résztvevőt is. Az adatcsere megoldható egy kijelölt szerverrel,
vagy az egyik játékos programja is elláthatja a szerver funkciót, illetve
elképzelhető akár felhő alapú megoldás is.

A játék megvalósítható például webalkalmazásként, mobil applikációként, vagy
desktop programként is.

## A program elvárt funkciói

  * Pálya beolvasása
  * Pálya megjelenítése
  * Játékosok mozgatása
  * Játékmenet kezelése (játék kezdete, végállapot felismerése, lépések szinkroban tartása)
  * Hálózati kommunikáckó
  * Powerupok kezelése

## Egyéb teendők a projekthez

  * Pályaelemek grafikáinak szerkesztése, vagy beszerzése
  * Pályafájlok generálása (kézzel, vagy programmal)

