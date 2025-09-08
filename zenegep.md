# Zenegép

A projekt célja egy olyan program létrehozása, amivel valós időben tudunk zenei alapokat (elsősorban hangminta alapú ismétlődő ritmusokat) előállítani.
A program működését talán a következő példán keresztül lehet szemléltetni. Tegyük fel, hogy a zenénk ütemmutatója 4/4 és minden ütemben az első
negyedben a lábdob, a második negyedben a lábcin, majd a pergő és végül megint a lábcin szól. (Ettől a bonyolult megfogalmazástól nem kell megijedni,
ez egy végtelenül egyszerű "tuc-tuc" dobalap.)

Ha külön képzeljük el a három ritmushangszer sávját, akkor például a következő módon tudunk egy ütemet szemléltetni (itt most nem negyedekre,
hanem nyolcadokra van bontva az ütem).

| 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 |
|---|---|---|---|---|---|---|---|
|**X**|     |     |     |     |     |     |     |
|     |     |**X**|     |     |     |**X**|     |
|     |     |     |     |**X**|     |     |     |

A programnak ezt a mintát kell újra és újra lejátszania, minden alkalommal lejátszva az adott hangszerhez tartozó hangmintát, illetve
ha egyidőben több hangszer is megszólal, akkor egyidőben a hozzájuk tartozó hangmintákat. Természetesen minden hangot tudnunk kell ki-
és bekapcsolni, hogy másfajta ritmusokat is be tudjunk állítani, illetve számos egyéb variáció is elképzelhető az változatosabb
hangzáshoz.

A programot akár desktop, akár mobil alkalmazásként el lehet készíteni, esetleg webes megvalósítás is elképzelhető.

## A program elvárt funkciói

  * Ritmusok bevitele, tehát annak beállítása, hogy egy adott időpontban az adott sávhoz tartozó hangszer megszólaljon-e, vagy ne.
  * Tempó szabályozása.
  * Lejátszás indítása, megállítása.
  * Annak jelzése, hogy az ütemen belül hol tartunk.
  * A főritmustól eltérő ütemek beállítása (például be lehessen állítani, hogy minden 4. ütem egy kicsit eltérő legyen). Például legyen más színű az a mező, amelyik csak bizonyos ütemekben szól stb.
  * Az egyes sávok némítása akár lejátszás közben, akár azon kívül

## Egyéb teendők a projekthez

  * Hangminták felvétele, vagy gyűjtése

