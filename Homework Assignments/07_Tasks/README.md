# Basics of Programming
## 7. Othoni Gyakorló Feladatok

### Feladatok
#### 1. Feladt
1. Inicializáljon egy sztringet, egy másikat pedig olvasson be a scanf() megengedett karaktereket
felsoroló változatával. Próbálja ki a string.h standard függvényeit (sztring hosszának
meghatározása, sztring másolás, sztring hozzáfűzés, karakter keresése sztringben, rész-sztring
keresés, két sztring összehasonlítása).
2. Olvasson be egy sztringet, majd írja ki virágnyelven; azaz minden magánhangzót ‘v’ előtaggal
megismételve. Például: “alma” → “avalmava”. A beolvasáshoz használja a scanf() függvényt.
3. Olvasson be egy sztringet, és állapítsa meg, hogy palindróma-e; azaz visszafelé olvasva ugyanazt
a szót kapjuk-e. Próbálja meg ugyanezt a feladatot space-t is tartalmazó szövegre is megoldani.
Palindrómára példa: “Géza kék az ég”.
4. Az akasztófa játékot (4. feladat) tegye folyamatos működésűvé.

5. Szókitaláló játék.
Inicializáljon egy sztringtömböt. Ebből véletlenszerűen kiválasztva egyet, keverje össze a betűit és
mutassa meg a felhasználónak. A feladat kitalálni az összekevert betűkből az eredeti szót. A
felhasználó mondjon tippeket, a program válaszoljon: hanyadik karakter helyét találta el (a
Mesterlogika játék mintájára). A játék végén írja ki a helyes szót és azt, hogy hány tipp után találta
ki a felhasználó.
6. Olvasson be egy mondatot (az utolsó karakter ‘.’, ‘?’, vagy ‘!’). Keresse meg, hogy a mondatban:
a) a mondatkezdő karakteren kívül van-e nagybetű és az hanyadik,
b) van-e speciális karakter vagy szám, és az hanyadik.


1. Írjon programot, amely kiszámítja egy ellenőrzötten beolvasott egész szám négyzetét. Az egyes
részfeladatokat külön függvényben valósítsa meg!
2. Írjon C programot, ami meghatározza egy ellenőrzötten beolvasott szám számjegyeinek az
összegét.
3. Az 5. feladat mintájára írjon olyan C programot, amely N ellenőrzött beolvasását követően kiírja
- N-ig az összes tükörszámot;
- az első N db tükörszámot;
- az N-jegyű tükörszámokat.
Tükörszám az, amelyik megegyezik a fordítottjával.
4. Az összes N-jegyű Armstrong-szám kigyűjtése. Armstrong-számnak nevezünk egy n jegyű
számot, ha minden számjegyét az n-edik hatványra emelve és összeadva, az eredeti számot kapjuk.
Ilyenek az egyjegyű számok és 153; 370; 371; 407; 1634; 8208; 9474; stb.

Számjegyek száma
beolvas n
db<-0
amig n<>0 végezd el
    db<-db+1
    n<-[n/10]
ciklus vége
kiír fb

Számjegyek összege
beolvas n
osszeg<-0
amig n<>0 végezd el
    osszeg<-osszeg+n%10
    n<-[n/10]
ciklus vége
kiír osszeg

Szám megfordítása
beolvas n
ford<-0
amig n<>0 végezd el
    ford<-ford*10+n%10
    n<-[n/10]
ciklus vége
kiír ford

5. A 4. gyakorlat rajzoló algoritmusait valósítsa meg függvényként. Pl. az N magasságú háromszög
kirajzolását megvalósító program kódja:

#include <stdio.h>
void haromszograjzolo(int magassag);

int main() {
    int m;
    printf("Adja meg a háromszög magasságát: ");

    scanf("%d", &m);
    haromszograjzolo(m);
    return 0;
}
void haromszograjzolo(int magassag) {
    int sor, i;
    for (sor=1; sor<=magassag; sor++) {
        for (i=1; i<=magassag-sor; i++) printf("%c", ' '); // space kiírása
        for (i=1; i<=sor+(sor-1); i++) printf("%c", '*'); // *-ok kiírása
        printf("\n"); // sortörés
    }
    return ;
}
6. Vegye elő a korábbi gyakorlatokon fejlesztett Kalkulátor programot. Módosítsa úgy, hogy a
végrehajtandó aritmetikai műveletek eredményét külön függvényekben számítsa ki.
7. Írjon C programot, amely külön függvényben ellenőrzött módon beolvas egy hatványalapot, ill.
egy kitevőt. Írja meg a hatványozást megvalósító függvényt.