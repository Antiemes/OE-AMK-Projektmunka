# Túlbonyolított dobókocka

Az *overengineering* nagyjából azt jelenti, hogy valamilyen (sok esetben egyszerű) feladatra
szükségtelenül komplikált megoldást dolgozunk ki. Magyarul talán túlbonyolítottnak lehetne
lefordítani. A projekt célja a társasjátékokhoz használható egyszerű dobókocka túlbonyolítása
informatikai eszközökkel. A felületet, ahova a kockát dobhatjuk, egy alkalmas pozícióban
rögzített kamera figyeli és képfeldolgozási / gépi tanulási módszerekkel felismeri
a kocka állását.

A projekt mind PC-n, mind mobiltelefonon megvalósítható. Mindkét esetben az OpenCV képfeldolgozási könyvtár használata ajánlott.

## A program elvárt funkciói

  * A kameráról érkező képfolyam fogadása, élőkép mutatása.
  * Kamerából érkező képfolyam helyettesítése képpel / videóval (reprodukálható tesztekhez lesz hasznos).
  * A kocka felismerése és jelölése a képen.
  * Dobási esemény felismerése.
  * Dobott szám felismerése, annak kijelzése. (Fontos, hogy a program egy dobást csak egyszer érzékeljen.)
  * Egyidőben több kocka felismerése.
  * Valamilyen dobókocka alapú játék megvalósítása, az ott előforduló kombinációk felismerése, a játékmenet követése.

## Egyéb teendők a projekthez

  * Kamera / telefon rögzítésének megoldása.
  * Teszt képek / videók felvétele (minden kockaoldalról többféle pozícióban és
    szögben, eltérő fényviszonyok mellett, esetleg több különböző kockával).

