# Megoldók készítése és összehasonlítása a Szózat játékhoz

A [Szózat](https://szozat.miklosdanka.com/) a [Wordle](https://www.nytimes.com/games/wordle/index.html)
magyar megfelelője. A játékban minden nap egy-egy 5 betűs magyar szót kell megfejteni.
Minden próbálkozáskor egy értelmes magyar szót kell beírni, a program pedig színekkel
jelzi, hogy melyik betűket találtuk el. A jó helyen eltaláltak zöldek,
a szóban máshol szereplők pedig sárgák lesznek. A kétjegyű betűk (sz, cs stb.)
is egy betűnek számítanak, a kettőzöttek viszont kettőnek. (A weblap az első
megtekintéskor megmutatja a példával is illusztrált játékszabályt.)

A projekt célja különböző (de legalább egy egyszerű és egy összetettebb)
megoldó készítése a játékhoz, valamint ezek tesztelése és összehasonlítása.
Természetesen ehhez magát az alapjátékot is meg kell valósítani úgy, hogy
az automatizált megoldás minél egyszerűbb legyen (tehát például függvénykönyvtár
formájában).

Mindkét megoldó és maga az alapjáték is egy szótárból dolgozhat.
A "buta" megoldó egy fix kezdőszó után leszűkítheti a teljes szótárat
(például ha eltaláltunk egy betűt, akkor csak azokat a szavakat hagyja meg,
amikben ez szerepel) és a kiszűrt szavakból akár véletlenszerűen
is választhat. A szűkítést természetesen lehet finomítani azoknak
a betűknek a kizárásával, amikről kiderült, hogy biztosan nem szerepelnek
a szóban, illetve a megtalált betűk pozícióját is érdemes felhasználni.
Egy okosabb megoldó a fennmaradó szavakból sem véletlenszerűen, hanem
valószínűségi alapon választ.

A megoldók elkészítése utái feladat azok tesztelése, az egyes szűkítések
hatásának vizsgálata.

## A program elvárt funkciói

  * Alapjáték elkészítése (csak a szótárban szereplő szavak elfogadása,
  találatok visszajelzése). Az alapjátéknak olyannak kell lennie, hogy ahhoz könnyen lehessen illeszteni
  a megoldót.
  * Buta megoldó elkészítése.
  * Szűkítések implementálása az egyre okosabb megoldók felé.
  * Megoldók tesztelése, adatok kiértékelése.

## Egyéb teendők a projekthez

  * Szótár elkészítése például egy általános szótár fájl szűrésével, vagy weben elérhető játék szótárának kinyerésével.
  * Stratégiák megalkotása.

