# Basics of Programming
## 5. Otthoni Gyakorló Feladatok

### Feladatok
#### 1. Feladt
- Inicializáljon egy sztringet, egy másikat pedig olvasson be a ```scanf()``` megengedett karaktereket felsoroló változatával.
    - Próbálja ki a ```string.h``` standard függvényeit (sztring hosszának meghatározása, sztring másolás, sztring hozzáfűzés, karakter keresése sztringben, rész-sztring keresés, két sztring összehasonlítása)!

#### 2. Feladt
- Olvasson be egy sztringet, majd írja ki virágnyelven, azaz minden magánhangzót ‘v’ előtaggal
megismételve.
    - Például: ```“alma” → “avalmava”```.
    - A beolvasáshoz használja a ```scanf()``` függvényt.

#### 3. Feladt
- Olvasson be egy sztringet, és állapítsa meg, hogy palindróma-e, azaz visszafelé olvasva ugyanazt a szót kapjuk-e.
    - Próbálja meg ugyanezt a feladatot space-t is tartalmazó szövegre is megoldani.
    - Palindrómára példa: ```“Géza kék az ég”```.

#### 4. Feladt (Szókitaláló játék)
- Inicializáljon egy sztringtömböt.
- Ebből véletlenszerűen kiválasztva egyet, keverje össze a betűit és mutassa meg a felhasználónak.
- A feladat kitalálni az összekevert betűkből az eredeti szót.
- A felhasználó mondjon tippeket, a program válaszoljon:
    - hányadik karakter helyét találta el (a Mesterlogika játék mintájára).
- A játék végén írja ki a helyes szót és azt, hogy hány tipp után találta ki a felhasználó.

#### 5. Feladt
- Olvasson be egy mondatot (az utolsó karakter ‘.’, ‘?’, vagy ‘!’).
- Keresse meg, hogy a mondatban:
    - a mondatkezdő karakteren kívül van-e nagybetű és az hányadik,
    - van-e speciális karakter vagy szám, és az hányadik.

#### 6. Feladt
- Töltsön fel egy $10$ elemű tömböt $10$ és $100$ közé eső véletlenszámokkal.
- Keresse meg ebben a tömbben:
    - a legkisebb prímszámot,
    - a legnagyobb négyzetszámot.

#### 7. Feladt
- Keresse meg az Interneten a férfi teniszezők világranglistáját (csökkenően rendezett sorozat).
- Tárolja el a pontszámokat tömbben és végezzen kereséseket.
- Implementálja a lineáris keresés és a logaritmikus keresés algoritmusait.
    - Próbálja ki a standard C ```bsearch()``` függvényt.
```C
// Összehasonlító függvény növekvő int sorozat esetén
int comparefunction(const void * a, const void * b)
{
    return *(int*)a - *(int*)b;
}

// bsearch() használata int sorozat esetén
int* item = (int*)bsearch(&searchkey, array, size, sizeof(int), comparefunction);

if( item != NULL )
    printf("Keresett elem: %d, sorszáma: %d\n", *item, item - array + 1);
else
    printf("Nem talált\n");
```

#### 8. Feladt
- Adottak egy egyetemi hallgató eredményei 6 félévre vonatkozóan (féléves tanulmányi átlagok)
időrendben.
- Keresse meg, hogy melyik félévben volt a hallgató tanulmányi eredménye $4.5$ fölött.
- Figyelem!
    - Azt az esetet is kezelje, ha nem volt ilyen félév, és azt is ha több ilyen félév volt.

#### 9. Feladt
- Keresse meg az Interneten a Forma1 világranglistát (csökkenően rendezett sorozat).
- Tárolja el a pontszámokat tömbben, növekvő sorrendben és végezzen kereséseket.
- Implementálja a lineáris keresés és a logaritmikus keresés algoritmusait.
    - Próbálja ki a standard C ```bsearch()``` függvényt.
- Hányadik a listában az a versenyző, akinek a pontszáma éppen fele annyi, mint a legmagasabb pontszám.
- Azt az esetet is kezelje, amikor nincs olyan pontszám, ami megfelel a feltételnek.

#### 10. Feladt
- $1990$ és $2020$ között hányadik év volt az első szökőév.

#### 11. Feladt
- Tekintsük a pitagoraszi számhármasokat $1$-től $100$-ig.
- Ezek azok a pozitív egész számokból álló számhármasok, amelyek lehetnek egy háromszög oldalai, azaz teljesül rájuk a háromszög egyenlőtlenség: $a < b < c$ és c$ ≤ 100$.
    - Melyik az a számhármas, amelyikre igaz, hogy az $a$, $b$ és $c$ közötti különbség rendre $10$.
    - Megoldás: $52$ db ilyen számhármas van és a $20$. a keresett eset.