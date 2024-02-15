# Tranziens jelek vizsgálata Arduinoval

Egy kontaktus átváltása (például egy kapcsoló, vagy relé ki- vagy bekapcsolása) soha nem
az áramkör egyszeri nyitása, vagy zárása, hanem ezek gyors ismétlése során létrejövő
tranziens folyamat (prellezés). A feladat ennek a jelenségnek a
vizsgálata Arduino segítségével, lehetőleg automatizáltan.

Lehetséges elrendezés: Az Arduino egy mini szervomotort vezérel, amivel időnként be- vagy
kikapcsolja a kapcsolót. (Használható két szervomotor is; az egyikkel be,
a másikkal a kikapcsoljuk a kapcsolót.) A kapcsoló ugyancsak az Arduinora van
kapcsolva, így az nyomon tudja követni, hogy pontosan hogy zajlott le a folyamat (tehát az átkapcsoláshoz
képest mikor kapcsolt át ténylegesen a kapcsoló, mikor váltott vissza, mikor változz megint vissza stb.)

Egy másik tranziens jelenség az izzólámpa be- és kikapcsolása, ahol számunkra
az izzószál áramának / ellenállásának változása az érdekes. Itt hasonló módon Arduino tudja be- és
kikapcsolni az izzót, aminek az árama plusz egy ellenállás beépítésével egyszerűen mérhető.

A begyűjtött adatokat aztán statisztikai módszerekkel fel lehet dolgozni.
