# Basics of Programming
## 1. Otthoni Gyakorló Feladatok

### Feladatok
#### 1. Feladt
- Írjon C programot, amely kiszámítja a háromszög területét oldalainak megadásával!
    - Használja a Hérón képletet: $t^2 = s * (s - a) * (s - b) * (s - c)$, ahol $a, b, c$ a háromszög oldalainak a hossza és s a kerület fele!
    - Ügyeljen a változók típusára!
    - A terület meghatározásához használja a négyzetgyökvonást végrehajtó függvényt: ```double sqrt(double)```!
    - Ennek deklarációját a ```math.h``` standard header állomány tartalmazza.

#### 2. Feladt
- Készítsen C programot, amely bekéri egy téglatest három oldalának hosszát és kiszámítja annak felszínét ($A = 2 * (a * b + a * c + b * c)$) és térfogatát ($V = a * b * c$)!
    - A felszín számításánál ügyeljen a helyes zárójelezésre!

#### 3. Feladt
- Írjon C programot, amely beolvas egy valós (```double``` típusú) számot és visszaadja a hozzá legközelebb eső kisebb ill. nagyobb egész számot.
    - Felhasználandó függvények: 
        - ```double ceil(double)```
        - ```double floor(double)```

#### 3. Feladt
- Írjon C programot, amely beolvas két egész számot, és kiírja az osztás eredményét az alábbi formában: ```osztandó / osztó = hányados, maradék x```.
- Ugyanezt oldja meg valós (```double``` típusú) számokkal is.
    - Az osztási maradék kiszámításához használja a ```math.h``` ```double fmod(double, double)``` függvényét!