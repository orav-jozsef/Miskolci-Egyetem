# Basics of Programming

## 2. ZH

### Kritériumok
Az elkészített feladat akkor elfogadható, ha:
- hiba nélkül lefordul (warning sem lehet) és futásidejű hiba nélkül lefut,
- az elvárt eredményt állítja elő,
- a feladathoz illeszkedő algoritmust helyesen alkalmazza,
- nem használ globális változót,
- a kód tabulált, jól olvasható; a változónevek beszédesek,
- a kód megfelel a feladatleírásnak,
- ellenőrzött adatbeolvasásnál a beolvasás sikerességét és a beolvasott érték helyességét is ellenőrzi,
- a tömb méretét kifejező konstans csak a változó deklarációs részben szerepel.


### Feladat
- Írjon C programot, amely megfelelő típusú és méretű egydimenziós tömbben nyilvántartja 10
hallgató zh eredményét: 38, 24, 12, 27, 22, 10, 32, 29, 26, 15.
    - Ezeket programból inicializálja.
- A dolgozat összpontszáma 40.
- Implementálja az alábbi részfeladatokat:
    1. Olvasson be ellenőrzött módon egy egész számot 20-25 között. Ez lesz a dolgozat sikerességének küszöbértéke.
    2. Hány hallgató dolgozata sikerleten? Ez az érték hány százaléka az összes dolgozatnak?
    3. Írja ki a pontszámok sorozatát úgy, hogy minden pontszám mellé zárójelben írja ki, hogy hány pont hiányzik a sikerességhez. A sikeres dolgozatok esetén 0.

### Példa
#### Input:
```
$>22
```
#### Output:
```
Sikertelen dolgozatok száma: 3, 30%
Pontszámok: 38 (0), 24 (0), 12 (10), 27 (0), 22 (0), 10 (12), 32 (0), 29 (0), 26 (0), 15 (7)
```