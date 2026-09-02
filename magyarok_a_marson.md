# Magyarok a Marson (két különálló feladatra bontva)

A [Magyarok a Marson](https://www.magyarokamarson.hu/weblap2026/index.php)
(várhatóan) 2027 áprilisi versenyére egy olyan távirányítható
járművet kell építeni, ami optikai kóddal működő kapukon tud áthaladni.
A megoldandó két részfeladat magának a járműnek a kidolgozása és a
kapuk nyitása gépi látással.

A járművel kapcsolatos részletes specifikáció a verseny honlapján található.
Röviden 18x18x18 cm-es maximális méret, megadott típusú motortípusból akárhány
darab, rádió távirányítás megadott típusú modullal. Értelemszerűen kell
valamilyen felépítmény, ami például 3D nyomtatással készülhet (de ez nem követelmény),
valamilyen motormeghajtó elektronika és a tápfeszültséget is biztosítani kell
valamilyen forrásból (leginkább akkumulátorból), de ezekben minden csapat szabad kezet kap.
A járműhöz tartozik még egy távirányító is. Ennek elkészítése is a csapat feladata.

## Megvalósítandó feladatok

  * Fő felépítés kigondolása (hány és mekkora kerék legyen, kormányzás megoldása stb.)
  * Mechanikai elemek kidolgozása (ez valósínűleg 3D tervezést és 3D nyomtatást fog jelenteni)
  * Elektronikai elemek kiválasztása, beszerzése, bekötése, mechanikai elrendezése (motormeghajtó, rádió modul, vezérlő egység)
  * Vezérlő egység programozása (rádió jelek vétele, motorok meghajtása)
  * Hasonló feladatok megtervezése, megvalósítása a távirányító esetében (nyomógombok, potméterek, 3D tervezés, nyomtatás, vezérlő egység, rádió modul stb.)

A kapuk nyitása lényegében
4 db LED villogásának felismeréséből, majd a kód egy más formában történő visszajátszásából
áll. Ennek a részfeladatnak a célja tehát a kódfelismerés. Ez megoldható akár a videó
WiFi-n történő továbbításával, akár helyben történő feldolgozással, de mindenképpen
olyan módszer szükséges, hogy a robot a ráhelyezett egységet könnyen elbírja.
A kapukon 4 db fehér fényű LED található, amik egy-egy bitet jelképeznek. Egy-egy 4 bites
állapot 200 ms-ig tart. Maga a kód F szimbólummal indul (minden LED világít), majd 3
változó érték látható, majd megint F és így tovább. A részletes protokoll, a kapuk méretei és
egy tesztvideó a verseny weblapján található.
A rendszer teszteléséhez véletlenszerű, vagy fix kódot adó kaput fogok tudni biztosítani.
Ez színben és a LED-ek fényerejében is biztosan különbözni fog a versenyen szereplő kaputól,
de a tesztekhez megfelelhet.

## Megvalósítandó feladatok

  * Architektúra kidolgozása (videó továbbítás, vagy helyben feldolgozás, milyen hardver és szoftver eszközökkel)
  * Képfeldolgozási megoldás (például OpenCV, vagy teljesen saját megoldás)
  * Tesztelés (tesztkörnyezet kialakítása, tesztek kiértékelhetőségének vizsgálata, majd kiértékelése)

## Egyéb teendők a projekthez

Ez egy rendkívül összetett feladat. A versenyen egy csapat legfeljebb 5 főből állhat, ennek
megfelelően (ha a teljes rendszert meg szeretnétek valósítani), akkor 2+3, vagy 3+2
összeállításban tudtok dolgozni. A gépi látás részfeladat nehezebb, viszont a jármű egyes
részfeladatai jobban szétoszthatóak. Ha maga a verseny a fő cél, akkor a leghatékonyabb
valószínűleg egy olyan összeállítású csapat lenne, ami vegyesen tartalmaz informatikus,
villamosmérnök és gépészmérnök hallgatókat is. Ekkor a szervezés is a feladatmegoldás
fontos részévé válik.

