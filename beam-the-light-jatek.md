# Beam the light játék

A projekt célja egy hálózati multiplayer játék megvalósítása. A játék célja lézersugarak irányítása tükrök segítségével egy négyzetrácson egy, vagy több cél felé.
A rács bármely pontja lehet:

 * egy játékos kezdőpontja (innen indul fel, le, jobbra, vagy balra az adott játékos lézere),
 * célmező (ide kell irányítani a lézert),
 * akadály (minden irányból elnyeli a lézert),
 * tükör (45 fokban áll és visszaveri a lézert).

A játékban minden pályán előre meghatározott az egyes játékosok célmezője, vagy
a közös célmező, illetve előre lerakott akadályok, vagy tükrök is lehetnek a
játékmezőn. A kezdőpont, illetve a lézer iránya lehet előre meghatározott, a
játékos által meghatározott, vagy akár mozgatható is. A játékosok hálózati
kapcsolaton csatlakoznak a játékhoz és felváltva léphetnek. Egy lépéssel
lerakható egy akadály, vagy tükör, esetleg a kezdőpont mozgatható. Az a játékos
nyer, akinek a lézere legelőször eléri a célmezőt.

Látható, hogy a játékmenet nem lett minden részletében specifikálva: Ennek
részletes kidolgozása a csapat feladat (lehetőleg úgy, hogy a játék kiegyensúlyozott
legyen és ne lehessen például a játék elején egyetlen tükör lerakásával nyerni).
Elképzelhető olyan verzió, ahol az első néhány lépéskor még nem aktív a lézerforrás,
vagy ahol először még csak akadályokat tudunk lerakni. Érdekes lehet egy olyan
szabály is, ahol a különböző lézerek 90 fokos találkozásakor azok felcserélődnek
(mintha mindkettő eltérítené a másikat).

## A program elvárt funkciói

  * Pontos játékmenet megalkotása.
  * Hálózati kapcsolat létesítésének kidolgozása (például az egyik játékos a szerver is egyben, a többi játékosok
  a kliensek, vagy külön szerver van).
  * Kommunikációs megoldás / protokoll kidolgozása.
  * Játékmenet kezelése / kijelzése (játékosok sorrendje, ki következik).
  * Lépés kezelése (például ne tudjunk felülírni egy akadályt, ha azt a játékszabály tiltja stb).
  * Játéktábla szinkronban tartása a játékosok között (mindenkinek ugyanazt az állást kell látnia).
  * Lézer útjának kiszámítása, kijelzése.


## Egyéb teendők a projekthez

  * Az egyes játékszabály verziók tesztelése, akár papíron.
  * Pályák készítése.

