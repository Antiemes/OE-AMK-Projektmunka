# Módosított sakk

A projekt célja egy olyan, módosított sakkjáték elkészítése, ahol a sakk eredeti
szabályainak egy része megmarad, mások megváltoznak. A módosított játékban
mindkét játékos választható számú azonos típusú bábuval játszhat, illetve
a játékmező mérete is változtatható. A lehetséges beállítások lehetővé tennék például
a klasszikus "parasztháborút" (8 gyalog 8 gyalog ellen), de érdekes lehet például
egy csak lovakból álló összecsapás, vagy kevesebb erősebb bábu több gyengébb ellen stb.
A nyerés / vesztés definiálása a csapat feladata. (Például az egyik játékos elveszítette az összes
bábuját, vagy az egyik játékos egy, vagy meghatározott számő bábuja elérte a tábla végét stb.)
A játékot kétszereplős multiplayerként kell elkészíteni.


## A program elvárt funkciói

  * Játéktípus és táblaméret beállítása.
  * Hálózati kommunikáció kidolgozása (az egyik program a szerver, hozzá
    csatlakozik a kliens, vagy mindketten egy közös szerverhez csatlakoznak
    stb.)
  * Játékmenet vezérlése (ki következik, lépés validálása, játéktáblák szinkronban tartása).
  * Nyerés / vesztés felismerése.
  * Patthelyzet felismerése. (Olyan állás, ami már volt egyszer, illetve
  amikor a soron következő játékos lépésképtelenné válik.)

## Egyéb teendők a projekthez

  * Játékszabályok megalkotása.
  * Játékszabályok validálása tesztjátékokkal.

