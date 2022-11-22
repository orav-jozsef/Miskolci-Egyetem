# Basics of Programming
## 8. Otthoni Gyakorló Feladatok

### Feladatok
#### 1. Feladt
- Írjon C programot a másodfokú egyismeretlenes egyenletek megoldásához.
Az ilyen egyenletek általános alakja:
    - $ax^2 + bx + c = 0$, ahol $a$, $b$ és $c$ konstansok.
    - Megoldása:\
        $x_{1,2}=\dfrac{-b\pm\sqrt{b^2-4ac}}{2a}$
        - Ha $a = 0$ de $b$ és $c$ nem $0$, az egyenlet elsőfokú, megoldása:\
        $x = \dfrac{-c}{b}$.
        - Ha $c = 0$ de $a$ és $b$ nem $0$, az egyenlet hiányos, megoldásai:\
        $x1 = 0$, $x2 = \dfrac{-b}{a}$.
        - Ha $b = 0$ de $a$ és $c$ nem $0$, az egyenlet tiszta másodfokú, megoldásai:\
        $x1,x2 = \pm\sqrt{\dfrac{-c}{a}}$
        - Ha mindhárom konstans $0$, akkor bármely szám megoldás.
        - Ha $a$ és $b$ $0$, viszont $c$ nem, akkor nincs megoldás.
    - A megoldóképletben a gyök alatti kifejezés a másodfokú egyenlet diszkriminánsa.
        - Ha $d > 0$, az egyenletnek két valós gyöke van.
        - Ha $d = 0$, az egyenletnek egy valós gyöke van ($x1 = x2$).
        - Ha $d < 0$ az egyenletnek két komplex gyöke van.
    - Struktúrák használata azért szükséges, mert a valós és komplex gyökök számítását végző fv több értéket kell visszaadjon.
    - Egy komplex számot leíró struktúra definíciója:
    ```c
    struct komplex {
        double valos;
        double kepzetes;
    };
    ```

#### 2. Feladt
- Egy egyetemi oktató 5 csoportba oszt szét 150 db ZH dolgozatot (max. 50 pont).
    - 0-25 pont elégtelen,
    - 26-32 pont elégséges,
    - 33-39 pont közepes,
    - 40-45 pont jó,
    - 46-50 pont jeles. 
- Készítsen C programot, amely elvégzi ezt a feladatot.

#### 3. Feladt
- Írja meg azt a C programot, amely megállapítja egy megadott dátumról, hogy hányadik napja az
évnek.
- Vegye figyelembe, hogy szökőévről van-e szó!
    - Készítse el az algoritmus fordítottját is:
        - ha adott, hogy hányadik napja az évnek, mondja meg, hogy melyik napról van szó. Pl. 2016-ban (szökőév) az év 60. napja február 29.
    - Készítse el azt a függvényt, amely megállapítja egy megadott dátumról, hogy helyes-e. Pl. 2016.01.32. hibás dátum.

#### 4. Feladt
- Olvassa be két síkbeli pont x és y koordinátáit.
- Számítsa ki a két pont távolságát (a Pitagorasz tétel alkalmazásával).
- A feladat megoldásához definiáljon saját Sikpont típust.

#### 5. Feladt
- Geometriai programban egy négyzetet az oldalhosszúságával és a bal felső csúcsának koordinátáival adunk meg.
- Határozza meg a négyzet középpontjának (az átló felezőpontjának) koordinátáit.

#### 6. Feladt
- Geometriai programban egy pont és egy kör egymáshoz viszonyított helyzetét vizsgáljuk.
- Állapítsa meg, hogy a megadott pont rajta van-e a megadott körvonalon, vagy azon belül, vagy azon kívül helyezkedik-e el.
- A pontot a koordinátáival adja meg, a kört pedig a középpont koordinátáival és a sugarával.