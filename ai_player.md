# AI játékos gépi látással

A projekt célja egy olyan program elkészítése, ami helyettünk tud játszani valamilyen
egyszerű játékkal úgy, hogy annak belső adataihoz nem fér hozzá (mint mondjuk
eggy sakkprogram), hanem csak a képernyőt látja. Erre a célra
[ezt](https://cdn-factory.marketjs.com/en/ant-smash/index.html) a
játékot választottam ki, ahol hangyák invázióját kell megakadályozni kattintásokkal.
A programnak tehát fel kell ismernie a hangyákat és mozgania kell az egeret.
Az igazán kidolgozott verzió pedig magát a játékmenetet is tudja kezelni.

A feladat jellege miatt ez a projekt leginkább desktop alkalmazásként képhelhető el.
A felismeréshez klasszikus gépi látás (elsősorban OpenCV), vagy AI megoldás (pl. Yolo)
használható.

## A program elvárt funkciói

  * Képernyő beolvasása
  * Játékablak behatárolása, vagy eleve csak ennek a beolvasása
  * Hangyák pozíciójának felismerése
  * Kattintás események generálása

## Egyéb teendők a projekthez

  * Grafikai információ gyűjtése
  * A felismerő algoritmus tanítása
  * Tesztek futtatása

