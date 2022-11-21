# Basics of Programming

## 1. ZH

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
- Írjon C programot, amely egy fiktív ötöslottó sorsolást valósít meg.
    - Implementálja az alábbi részfeladatokat:
        1. A sorsolás eredményét peszeudorandom módon generálja (5 db egész szám 1 és 95 között, a számok nem ismétlődhetnek). Az eredményt megfelelő típusú és méretű egydimenziós tömbben tároljuk.
        2. Kérjen be a felhasználótól egy szelvénnyi (5 db) számot ellenőrzött beolvasással, ügyelve arra, hogy a korábbi kritériumoknak megfeleljenek, szintén tömb formájában tárolva.
        3. Írjuk ki a kisorsolt számokat.
        4. Írjuk ki a helyes találatokat és azok számát.

### Példa
#### Input:
```
Kerem toltse ki a szelvenyet:
$>1
$>2
$>-1
Helytelen ertek, kerem adjon meg ujat:
$>3
$>4
$>5
```
#### Output:
```
A het nyero szamai: 5 15 21 49 72
Az on altal eltalalt szamok: 5
On 1 szamot talalt el.
```