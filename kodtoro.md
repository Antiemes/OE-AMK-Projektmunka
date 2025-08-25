# Monoalfabetikus titkosítás automatikus megfejtése

A projekt célja monoalfabetikus titkosítással rejtjelezett szövegek automatikus
megfejtése. A monoalfabetikus (egybetű-helyettesítéses) titkosító úgy működik,
hogy minden betűt, esetleg az írásjeleket is egy adott (más) betűre, vagy
írásjelre cserél. A 26 betűs angol ábécé esetében elvileg 26! (körülbelül 400
kvadrillió) féle konkrét kulcs létezik, ennek ellenére ez a titkosító
viszonylag egyszerű módszerrel feltörhető a természetes nyelvek statisztikai
jellemzői miatt.

A feladat egy olyan program elkészítése, ami képes megfejteni egy monoalfabetikus
titkosíŧóval rejtjelezett magyar szöveget, kijelezve a köztes lépéseket is.

## A program elvárt funkciói

  * Szöveges (`.txt¸`) UTF-8 karakterkódú fájl beolvasása.
  * Statisztikák megjelenítése (betűk, egyéb karakterek, szóhosszok gyakorisága, mondatkezdő nagybetűk, írásjelek megléte stb.
  * Annak felismerése, hogy feltehetően egy magyar szöveg monoalfabetikus rejtjelezése (alapvetően a stasztikai kiértékelés alapján).
  * Többször ismétlődő, biztosra vehető szavak kigyűjtése, helyettesítése.
  * A megfejtett betűk alapján újabb szavak megfejtése (szótár segítségével).
  * Annak felismerése, hogy egy bizonyos ponton az eddigi megoldás helytelen. Visszalépés és más alternavítával való próbálkozás.
  * A megfejtett szöveg megjelenítése, elmentése, kulcs megjelenítése.

## Egyéb teendők a projekthez

  * Teszt szövegek előállítása (gyűjtéssel, illetve írással).
  * Titkosító elkészítése. (Megjegyzés: A többjegyű betűket karakterenként kell kódolni.)
  * Kiindulási betűstatisztika készítése.
  * Szótár előállítása a szavak megfejtéséhez.
  * Program tesztelése a szövegbázison.

