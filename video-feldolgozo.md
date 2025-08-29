# Automatikus videófeldolgozó online tananyagokhoz

A projekt célja az online tananyagok készítése feldolgozása közben felmerülő
repetitív feladatok automatizálása. Az ilyen típusú videófelvételek nagyrészt a
diasor egyes diáit mint állóképeket, illetve esetleg rövid animációkat, a
hangfelvételek pedig beszédet tartalmaznak.

A hangsáv feldolgozásának teljes mértékben automatizálható lépése a zajszűrés,
majd a hangerő egységes szintre hozása (normalizáció), végül kiegészítő
hangerő növelő módszerek (kompresszor, limiter) alkalmazása. Ezek a műveletek
az eredetire pontosan illeszkedő hangsávot eredményeznek, tehát az eredeti
hangsáv egy az egyben lecserélhető az így kapottra.

Szintén a hangsáv alapján végezhető el a hosszú (egy beállítható hosszúságúnál nagyobb)
szünetek, illetve az "ő-zés" felismerése és automatikus eltávolítása.
Az így kapott hangsáv természetesen már nem "passzol" az eredeti videósávhoz,
így minden olyan helyen, ahol a hangsávból egy részt törlünk, a videósávból is
ugyanennyit törölni kell (hogy megmaradjon a szinkron a kettő között).
Emiatt természetesen csak egy képkocka hosszának egész számú többszörösei
törölhetőek.

A fenti funkciók a konkrét vágóprogramtól függetlenül megvalósíthatóak, bár
elképzelhető a plugin verzió is. Egy, a vágást nagyban segítő funkció még
a diaváltások jelölése clip marker formájában. A különböző vágóprogramok
más-más fájlformátumból tudnak clip markert importálni, célszerű egy olyan
vágóprogramhoz tartozó formátumot választani, ami nyílt forráskódú, vagy
legalábbis ingyenesen használható.

## A program elvárt funkciói

 * Gyakori videófájlfájl-formátumok (de legalább az MP4) támogatása, azok
 olvasása és írása.
 * Manuális és batch üzemmód (például egy mappában az összes videófájl
 feldolgozása).
 * A kimeneti fájl nevének generálása az eredetiből (például a `valami.mp4`-ből
 `valami_processed.mp4`.
 * Csak a hangot érintő előfeldolgozási lépések (normalizáció, kompresszió,
 limitáció) elvégzése).
 * Szünetek felismerése, kivágása, a szünethossz beállítása.
 * Ő-zés felismerése, kivágása, algoritmus esetleges paramétereinek
 beállítása.
 * Kép-hang szinkron megtartása.
 * Diaátmenet-marker fájl generálása.

A projekt elkészíthető önálló programként, vagy pluginként valamilyen meglévő
nyílt forráskódú (pl. KDEnlive), vagy legalábbis ingyenes videószerkesztőhöz.

## Egyéb teendők a projekthez

 * Videó anyagok elkészítése, vagy beszerzése (mindenképpen több forrásból,
 több előadóval).
 * Ő-zések kigyűjtése, detekciós algoritmus készítése (például gépi tanulási
 módszerrel), annak tesztelése (fals-pozitív, fals-negatív).

