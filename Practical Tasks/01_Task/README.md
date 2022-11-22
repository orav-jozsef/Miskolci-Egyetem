# Object Oriented Programming
## 1. gyakorlat (Java)

### ***Elsajátítandó ismeretek***
1. Eclipse IDE megismerése, Javadoc generálás
2. Első Java projektek elkészítése, fordítás, futtatás (parancssorból is)
3. Ellenőrzött beolvasás (```Scanner```, ```BufferedReader``` objektumokkal)
4. Egydimenziós tömbök kezelése (deklaráció, inicializálás, tömb túlindexelés, inicializálatlan változóra hivatkozás, tömb mint fv argumentum)
5. Típuskonverzió (monotonitás vizsgálat: ```boolean``` ↔ ```int``` között nincs; faktoriális számítás: ```long float``` értékvesztéssel jár)

### ***Algoritmizálási feladatok, egydimenziós tömb kezelése***
> - A feladatok megoldása során a strukturált, top-down programfejlesztési alapelvet használjuk.
> - Figyeljék meg, hogy most minden metódus ```static```!
> - Magyarázat: csak egy osztályunk van, ami futtatható (van benne main metódus) és ebben az osztályban hívjuk a metódusokat anélkül, hogy az osztályt példányosítanánk.
> - Azaz a ```static``` metódusok nem objektumokhoz kötődnek, hanem az osztályhoz.
> - Amikor tömböt adunk át függvénynek argumentumként, a tömb méretét nem kell átadjuk, mert a tömb méretét a ```length``` tulajdonság mindig megadja.

### ***Feladatok***
#### 1. Feladat
- Adjon közelítést $\pi$ értékére ($3.1415926535$), az alábbi sorozatok első $1000$ tagjának kiszámításával.
- Melyik sor konvergál gyorsabban?
    - Leibniz-féle sor:
    $$\dfrac{\pi}{4} = 1 - \dfrac{1}{3} + \dfrac{1}{5} - \dfrac{1}{7} + ...$$
    - Wallis-formula:
    $$\dfrac{\pi}{2} = \dfrac{2}{1} * \dfrac{2}{3} * \dfrac{4}{3} * \dfrac{4}{5} * ...$$
- Adjon közelítést az Euler-féle $\mathrm{e}$ számra ($\mathrm{e} = 2.718 281 828$) az alábbi sorozat első $11$ tagjának kiszámításával:
$$\mathrm{e} = \sum_{n = 0}^{\infty}\dfrac{1}{n!} = \dfrac{1}{0!} + \dfrac{1}{1!} + \dfrac{1}{2!}$$
- A faktoriális számítást külön függvényben valósítsa meg!

#### 2. Feladat
- Állítsa elő az $1$ és $100$ közé eső számokból készíthető összes számpárt (a számpárok különböző számokból állnak).
- Számolja meg, hogy ezek közül hány számpárra igaz, hogy ikerprímek és írja ki ezeket a számpárokat a konzolra.
- Megoldás: $9$ ilyen számpár van.
Az ikerprímek olyan prímszámok, melyek különbsége $2$ (pl. $5$ és $7$ ikerprímek).

#### 3. Feladat
- Deklaráljon és inicializáljon egy $10$ elemű int tömböt és valósítsa meg az alábbi algoritmusokat külön metódusként:
    - tömbelemek kiírása
    - tömbelemek kiírása fordított sorrendben
    - páros számok átlagának kiszámítása
    - minimumkeresés
    - monotonitás vizsgálat (monoton növekvő-e a számsor)
    - növekvő rendezés minimum kiválasztással