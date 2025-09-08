# Tranziens jelek vizsgálata Arduinoval

Egy mechanikus kontaktus átváltása (például egy kapcsoló, ki- vagy
bekapcsolása) a valóságban soha nem úgy történik, hogy az áramkör egyszer nyit,
vagy zár; az átkapcsolás pillanatában az érintkező egy kis ideig "prellezik",
vagyis egyfajta rezgést végez, miközben egymás után többször nyitja-zárja az
áramkört. A feladat ennek a tranziens jelenségnek a vizsgálata Arduino
segítségével.

A vizsgálati áramkör rendkívül egyszerű: Egy Arduino fejlesztőkártya egyik GPIO portja
és a földkivezetés közé egy kapcsolót szerelünk, az Arduino a GPIO port állapotát figyeli
és méri, hogy az első átkapcsolást követően pontosan milyen folyamat zajlott le (mikor és hányszor
váltott állapotot a GPIO port, mielőtt stabilizálódott a végső állapot).

A GPIO port figyelését mindenképpen gyors módszerrel kell megoldani (capture funkció, vagy legalább
pin change interrupt). A begyűjtött adatokat statisztikai módszerekkel kell feldolgozni.
Ehhez a projekthez több egymással összedolgozó program megírására is szükség van.
Az Arduinon futó program felelős az időkritikus funkciókért, ami a PC-n futó
adatgyűjtő programmal kommunikál. Végül a felvett adatok elemzése egy harmadik program feladata lehet.

A projekthez egy Arduino Uno fejlesztőkártyát és többféle kapcsolót biztosítok.

## A program elvárt funkciói

  * Kapcsoló nyitásának / zárásának felismerése.
  * További be-ki, illetve ki-be átmenetek időpontjának feljegyzése.
  * Állandósult állapot felismerése.
  * Feljegyzett adatok továbbküldése az állandósult állapot kialakulása után. Az időkritikus mérés közben ne küldjünk semmit, kizárólag utána.
  * Kommunikációs protokoll, illetve fájlformátum kidolgozása.
  * Mérések elemzése.

## Egyéb teendők a projekthez

  * Mérési adatok szisztematikus gyűjtése (többféle kapcsoló, normál átkapcsolás, hirtelen átkacsolás stb).
