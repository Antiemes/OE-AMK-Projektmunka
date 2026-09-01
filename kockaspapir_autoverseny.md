# Autóverseny négyzetrácsos papíron

A négyzetrácsos autóverseny egy klasszikus társasjáték, amit papíron játszanak.
Minden autó egy bizonyos sebességvektorral rendelkezik, ami azt határozza meg,
hogy egy lépés során merre, illetve hány mezőt mozdul el (például két mezőt jobbra,
egyet fel). Minden lépésben a sebességvektor mindkét összetevője legfeljebb 1
egységgel változtatható meg.

A játék kezdetekor az autók a megadott startpontok valamelyikéről (például egymás mellől)
indulnak, kezdeti sebességük 0. Ezután következhet egy sebességváltoztatás, majd
egy annak megfelelő lépés az összes játékos részéről, majd egy újabb sebességváltoztatási
lehetőség újabb lépéssel stb.

A játékhoz tartozik még természetesen egy pálya is, aminek alakja tetszőleges lehet.
Az autók mindig bizonyos rácspontok között egyenes vonalban mozognak, a pálya viszont
finomabb felbontású is lehet. A cél végig az, hogy az autónk minél kevesebb lépés alatt
a célba jusson (esetleg adott számú kört megtegyen) anélkül, hogy a pálya falának ütközne.

A játék alapvetően hálózati multiplayer kivitelben képzelhető el, de ez esetleg egy,
vagy több (esetleg ügyesebb és kevésbé ügyes) gépi ellenfél megvalósításával
kiváltható.
Megvalósítható desktop, mobil, vagy webes alkalmazásként is.

## A program elvárt funkciói

  * Pálya tárolása (például képként)
  * Pálya beolvasása, megjelenítése
  * Lépések kezelése (például a következő rácspont kiválasztásával)
  * Játékosok mozgatása
  * Játékmenet kezelése (játék kezdete, végállapot felismerése, lépések szinkroban tartása)
  * Hálózati kommunikáckó
  * Falnak ütközés felismerése
  * Gépi ellenfelek elkészítése

## Egyéb teendők a projekthez

  * Pályaelemek grafikáinak szerkesztése, vagy beszerzése
  * Pályafájlok elkészítése

