# Basics of Programming
## 6. Otthoni Gyakorló Feladatok

### Feladatok
#### 1. Feladt
- Deklaráljon egy 10 elemű integer tömböt.
- Írjon függvényt, amely feltölti a tömb elemeit 1 és 5 közé eső véletlenszámokkal.
    - Írjon függvényt, amely visszaadja a sorozat móduszát (a legtöbbször előforduló elemét).
        - Hogyan kezelné azt az esetet, amikor többmóduszú a sorozat?
            - Például az 1, 1, 1, 2, 3, 4, 4, 5, 5, 5
        - sorozatban a leggyakrabban előforduló elemek az 1 és az 5, mindkettőnek azonos az előfordulási gyakorisága.
        - Vannak olyan sorozatok, ahol minden elem azonos gyakorisággal fordul elő (pl. egyszer, ha nincs az elemek között ismétlődés).
            - Ekkor azt mondjuk, hogy a sorozat móduszát nem lehet meghatározni.
        - Ezt az esetet is kezelje a program.
    - Írjon függvényt, amely kiírja a rendezett sorozatot.
    - Írjon függvényt, amely kiírja a sorozat statisztikáját táblázatos formában:
        - melyik elem hányszor fordul elő.
        - Például ha a sorozat elemei 1, 1, 1, 2, 3, 4, 4, 5, 5, 5, a statisztika így néz ki:
        ```c
        1 - 3 db
        2 - 1 db
        3 - 1 db
        4 - 2 db
        5 - 3 db
        ```

#### 2. Feladt
- Olvasson be egy szöveget.
- Írjon függvényt a szöveg kódolására (titkosítására), majd dekódolására.
- A feladatnak a szöveg nagybetűssé konvertálásához hasonlóan 3 lehetséges megközelítése van.

#### 3. Feladt
- Implementálja a 6. előadás sztringkezelő algoritmusait saját függvényként.
- Minden esetben próbálja ki a megfelelő standard függvényhívást is (sztring hosszának meghatározása, sztring másolás, sztring hozzáfűzés, karakter keresése sztringben, rész-sztring keresés).