# Általanos információk

## Időbeosztás, mérföldkövek

A félév során **csapatban** **KELL** dolgozni. Egy csapat 2-3 főből állhat, amitől indokolt esetben felfelé igen, lefelé
semmilyen esetben sem tudunk eltérni. Egy fős csapat nem megengedett. A csapatok összeállítását a második héten lezárjuk.

A csapatok összeállításával párhuzamosan folyik a téma kiválasztása (lásd lentebb).

A csapatoknak 4 konzultáción kell részt venniük a félév során. Ezek az órarend szerinti időpontok közül kerülnek kiválasztásra, a félév során egyenletesen elosztva.

A félév során **dokumentáció** készítése szükséges (lásd lejjebb).

A féléves munkát egy közös, **személyes beszámoló zárja** (úgyszintén lásd lejjebb).

### Csapatok összeállítása

A csapatok összeállítása alapvetően a hallgatók feladata. Ezt egy online táblázat segítségével lehet megtenni,
aminek a linkje a Moodle-ben szerepel.
Értelemszerűen a "csapat sorszáma" oszlopba kell beírni
a csapat sorszámát. A táblázatot később letisztázom és a kimaradó emberekből (ha
lesznek) véletlenszerűen állítok össze csapatokat.

A csapatok összeállítását a **második hét végéig** le fogjuk zárni. **A táblázatban módosítani az második hét szerda 18:00-ig lehet**.
Ezt követően a kimaradó embereket önkényesen fogom csapatokba rendezni.

### GitHub regisztráció és meghívó

A féléves munkához szükség van a GitHub-ra történő regisztrációra is. Az ottani **felhasználónevet** úgyszintén be kell
írni ebbe a táblázatba. A csapatok véglegesítése után mindenkit meghívok az előre elkészített GitHub repositoryba (ehhez
kell tudnom a felhasználónevet). A meghívás után az illető nevét sárgára állítom. A meghívó elfogadását rendszeresen
ellenőrizni fogom és ennek alapán állítom az adott embert zöldre. Aki nem fogadja el a meghívót a **harmadik hét szerda 18:00-ig**,
az **aláírásmegtagadást kap**.

### Konzultációk

A félév során **4 konzultáció** szükséges, amit az órarendi időpontok közül választva, együtt, személyesen tartunk.

A konzultációk időpontja:
  * 1. konzultáció: **Szeptember 11.** (1. hét)
  * 2. konzultáció: **Október 9.** (5. hét)
  * 3. konzultáció: **Október 30.** (8. hét)
  * 4. konzultáció: **November 27.** (12. hét)

A konzultációk helye: K038, 9:50-10:35.

### Írásbeli beszámoló

Az írásbeli beszámolót a [szakdolgozat sablonban](https://amk.uni-obuda.hu/wp-content/uploads/2024/03/Szakdolgozat_sablon_2023.docx) kell elkészíteni. Minimális terjedelme 25 oldal. A beadási határidő december 5-e (utolsó oktatási hét hétfő).

## Témák

A következőkben a lehetséges választható témák kerülnek felsorolásra. Ezek nagyrészt nem
konkrét, minden tekintetben kidolgozott feladatok, hanem csak kiindulási alapok, amiknek több
konkrét kidolgozása is lehetséges. Így az esetek nagy részében több csapat is választhat hasonló témát.

[Túlbonyolított dobókocka](dobokocka.md)

[Megoldó logikai játékhoz](gamesolver.md)

[Tangram társasjáték számítógépes megvalósítása](tangram.md)

[Játék Arduinoval és OLED kijelzővel](arduino-jatek.md)

[Okos otthon megvalósítása NodeRed segítséglvel](okos-otthon.md)

[WiFi aktivitás mérése Raspberry Pi segítségével](wifi-aktivitas.md)

[Beszélő óra, beszélő konyhai időzítő, beszélő műszer](beszelo.md)

[Tranziens jelek vizsgálata Arduinoval](tranziens.md)

[Zenegép](zenegep.md)

[Diavetítő szimulátor](diavetito.md)

[Monoalfabetikus titkosítás automatikus megfejtése](kodtoro.md)

[Automatikus videófeldolgozó online tananyagokhoz](video-feldolgozo.md)

## Verziókövetés

A kurzus egyik célja a Git használatának elsajátítása. Ez azt jelenti, hogy ahelyett,
hogy a csapattagok a kódrészleteket például e-mailben, Messengeren stb. osztanák meg
egymással, a változásokat Git használatával követik. Ez egyben azt is jelenti, hogy
a Git repositoryban nem csak a kész, működő verziónak kell szerepelnie, hanem látszani
kell annak is, hogy a félév során mi történik.

A csapatoknak a készülő kód és az egyéb fájlok mellett a dokumentációt is ugyanebben a
GitHub repositoryban kell (verziókövetve) tárolniuk.

### A fejlesztői környezet beállítása a Githez

A fejlesztés első (vagy inkább nulladik) lépése a fejlesztőrendszer beállítása a Githez. A legtöbb
IDE képes a Gittel együttműködni, azonban mindegyiket egy kicsit máshogy kell beállítani. Egy
további lehetőség akár egy grafikus, akár az alap parancssoros Git kliens használata.

Addig senki ne kezdjen hozzá a fejlesztéshez, amíg a Git használata nem megy rutinszerűen.

### README.md

A repositoryban levő README.md fájl a projekt rövid összefoglalója.
Itt szerepelhet például:

 * A csapattagok névsora, Neptun kódja, esetleg elérhetősége
 * A projekt neve, elnevezése
 * A projektről néhány mondat, amiből képet kapunk arról, hogy mit csinál a csapat
 * A felhasznált technológiák, programnyelvek
 * Az előrehaladási napló (nagyobb mérföldkövek; mit csinált a csapat)

A README.md formátuma MarkDown, ami egy egyszerű szövegformázó (markup) nyelv.
Rövid leírás például [itt](https://www.markdownguide.org/basic-syntax/).

**A README.md naprakészen tartása elvárás a kurzus teljesítéséhez.**

### .gitignore

A .gitignore fájl arra való, hogy bizonyos fájlokat automatikusan figyelmen kívül
hagyjunk a verziókövetés során. Ezek például a projekt fordítása során létrejövő,
a forráskódból generált fájlok. Interneten számos példa lelhető fel ezzel kapcsolatban.
Egy kiindulási alap lehet például
[ez a gyűjtemény](https://github.com/github/gitignore).

**A .gitignore fájlnak az adott fejlesztőeszközhöz passzoló kitöltése elvárás
a kurzus teljesítéséhez.**

### Könyvtárstruktúra

A repositoryban külön könyvtárban kell elhelyezni a projekt forráskódját (és a
kapcsolódó egyéb fájlokat), a dokumentációt, illetve az egyéb állományokat.
Néhány példa:

 * **src**: A projekthez tartozó forráskódok
 * **firmware**: Az esetleges mikrovezérlős forráskódok
 * **docs**: Dokumentációk
 * **schematics**: Kapcsolási rajzok
 * **screenshots**: Képernyőképek

**A kurzus során elvárás a tiszta könyvtárszerkezet használata.**

### Commitok

A változásokat commitok formájában lehet a verziókövetőbe feltölteni. Minden
commithoz szükséges kitölteni a "commit message"-et is. A feltöltéshez
csak **NE** használjuk a "file upload" funkciót!

A csapatok a félév során **rendszeresen** kell, hogy commitokat készítsenek.
Mivel a "rendszeresen" szónak való megfelelést nehéz utólag elbírálni,
így a következő konkrét mérőszámok az irányadóak. Egy valós fejlesztés
során persze ennél minimum egy nagyságrenddel több commit szokott születni.

**A kurzus során elvárás, hogy legyen legalább 10 olyan hét, amikor ÉRDEMI
változás történik a repositoryban és ezt a commitok dátuma is tükrözi.**

**Szintén elvárás, hogy minden csapattag esetében legyen legalább 3-3 olyan hét,
amikor az adott csapattagnak ÉRDEMI commitja van.**

Érdemi commit lehet akár egy egyeztetésről szóló bejegyzés az előrehaladási
naplóban, vagy akár valamilyen, a projekthez kapcsolódó ötlet, vagy kísérlet nyoma
(fotó, rövid leírás stb) is.

