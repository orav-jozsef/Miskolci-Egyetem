# Basics of Programming
## 9. Otthoni Gyakorló Feladatok

### Feladatok
#### 1. Feladt
- A beolvasott könyv adatok eltárolása fájlban, majd a fájl kilistázása.
- A fájlból visszaolvasva az adatokat végezzük el az alábbi feladatokat, amelyeket külön függvényként implementálunk.
    1. Számoljuk meg hány könyv található a könyvtárban.
    2. Összesítsük a könyvtárban található könyvek árát.
    3. Keressük meg a legrégebbi / legújabb könyvet.
    4. Döntsük el h. egy adott című könyv szerepel-e a könyvtárban.

#### 2. Feladt
- Hozzon létre egy autó adatait tárolni képes struktúrát.
    - Hozzon létre egy $10$ autó adatait tároló dinamikusan lefoglalt tömböt.
    Definiálja a struktúrán elvégezhető alábbi műveleteket:
        - beolvasás,
        - kiírás,
        - 15%-os árleszállítás,
        - a legdrágább/legolcsóbb
        - autó megkeresése,
        - autók átlagárának kiszámítása,
        - megadott ár-értékhatárok közé eső autók megszámolása (pl.: $2 000 000$ Ft és $3 000 000$ Ft).
    - Tárolja el fájlban a beolvasott adatokat.
        - Listázza a fájl tartalmát, és az előző műveleteket a fájlból visszaolvasás után valósítsa meg.
    - Módosítsa az autó struktúra típust:
        - az árat összeg és devizanem formájában akarjuk megadni (beágyazott struktúra) (pl.: $20 000$ Euro, $2 000 000$ Ft).
        - Ennek megfelelően módosítsa a programban definiált funkciókat.

#### 3. Feladt
- A 12. előadás anyaga alapján készítsen mátrix műveleteket végző programot.
    - Két mátrix összeadása.
    - Két mátrix szorzása.
    - Mátrix transzponálása (sorok és oszlopok felcserélése).
    - Mátrix determinánsának kiszámítása.

#### 4. Feladt (Aknakereső játék)
- Egy 10x10-es játékmezőn helyezzünk el véletlenszerűen 20 darab, nem szomszédos aknát.
- A felhasználó 10szer tippelhet.
- Minden tipp után mondjuk meg, hogy talált-e.
- Számoljuk, hány aknát talált meg összesen.

#### 5. Feladt
- Készítse el a kő-papír-olló játék programját.
- Használjon enum típusú változót a válaszlehetőségek tárolásához.
- A felhasználó játszik a géppel.
- A program akkor álljon le, amikor a felhasználó már nem akar tovább játszani.
- Minden kör végén írja ki, hogy ki nyert.
- A játék legvégén pedig legyen statisztika:
    - ki hányszor nyert.
- *Segítség:*
```c
enum tipp {KO, PAPIR, OLLO}; //KO=0, PAPIR=1, OLLO=2

do {
    printf("Mit választasz?"); // felhasználó válaszát beolvasni, eltárolni ‘valasz’ változóban
    gep = rand()%3; //0-2 közötti véletlenszám
    // eldönteni ki nyert, tárolni
    // eredményt kiírni
    printf("Akarsz még játszani? ");
    scanf(" %c", &tovabb);
} while (tovabb=='i' || tovabb=='I');

// statisztika
```