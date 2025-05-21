# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

#### ✅ Mi a tesztelés célja? Mi nem az?

#### A tesztelés célja:
- Hibák felismerése: 
  - A tesztelés fő célja, hogy azonosítsa a szoftverben rejlő hibákat vagy anomáliákat.

- Minőségbiztosítás: 
  - A tesztelés segít a szoftver minőségének biztosításában, és megerősíti, hogy a rendszer a specifikációknak megfelelően működik.

- Megfelelőség ellenőrzése: 
  - Ellenőrzi, hogy a fejlesztett rendszer megfelel-e az üzleti követelményeknek, és hogy a felhasználói igényeknek is eleget tesz.

#### Mi nem a tesztelés célja:
- A szoftver biztosítéka: 
  - A tesztelés nem garantálja a hibamentességet, csak a hibák felfedezésére szolgál.

- Kódolás vagy fejlesztés helyettesítése: 
  - A tesztelés nem a kód megírását vagy a fejlesztési folyamatokat helyettesíti, hanem azok után következik.

- A fejlesztési hibák egyedüli forrása: 
  - A tesztelés nem célja az egyes fejlesztői hibák kiderítése, inkább a rendszer átfogó hibáinak feltárása.

##

#### ✅ Mik a tesztelési alapelvek?

1. A tesztelés hibákat mutat, nem a hibamentességet  
A tesztelés kimutathatja a hibák jelenlétét, de soha nem garantálja, hogy a rendszer hibamentes. A hibamentesség igazolása nem lehetséges.  

2. Kimerítő tesztelés nem lehetséges  
Minden lehetséges esetet lefedő tesztelés kivitelezhetetlen. Ehelyett a tesztelési erőforrásokat kockázatelemzéssel és prioritásokkal kell fókuszálni.  

3. Korai tesztelés előnyei  
A hibák korai megtalálása időt és költséget takarít meg. Ezért a tesztelési tevékenységeket minél előbb, a fejlesztési életciklus elején el kell kezdeni.  

4. Hibafürtök jelensége  
A hibák gyakran néhány modulban koncentrálódnak. A hibafürtök azonosítása segíthet a hatékonyabb tesztelésben.  

5. Féregirtó paradoxon  
Az ismétlődő tesztek idővel kevésbé hatékonyak. Új hibák feltárásához a teszteket frissíteni, bővíteni kell.  

6. Tesztelés a körülmények függvényében  
A tesztelési megközelítések a projektek jellegétől függően változnak, például biztonságkritikus rendszerekben más szempontok érvényesülnek, mint e-kereskedelmi alkalmazásokban.  

7. Hibamentesség mítosza  
Minden hiba megtalálása és javítása sem garantálja a rendszer sikerét. Egy hiba nélküli, de nehezen használható rendszer is megbukhat a gyakorlatban.

##

#### ✅ Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?

- Az egységtesztelés a szoftvertesztelés egy szintje, amelyben az alkalmazás legkisebb, önállóan tesztelhető egységeit ellenőrzik. Az egységtesztek célja annak biztosítása, hogy az egyes komponensek megfelelően működjenek a tervezett funkcióik szerint.

- Az egységtesztek írásáért általában a fejlesztők a felelősek, mivel ők rendelkeznek a legnagyobb ismerettel az adott modulok vagy komponensek belső működéséről. Az egységtesztelés gyakran a fejlesztési folyamat része, és sok esetben automatizáltan hajtják végre.

##

#### ✅ Mik a tesztszintek, és mi a különbség köztük?

#### A tesztszintek hierarchikus rendszerben vannak rendezve:

- Egységtesztelés (Unit Testing): 
  - A kód legkisebb egységeinek tesztelése.

- Integrációs tesztelés (Integration Testing): 
  - Különálló egységek összekapcsolása, hogy az együttműködésük megfelelő legyen.

- Rendszertesztelés (System Testing): 
  - Az egész rendszert tesztelik annak érdekében, hogy biztosítsák, hogy az megfeleljen az összes specifikációnak.

- Rendszer integrációs:
  - A rendszerintegrációs tesztelés a rendszerek és mikroszolgáltatások közötti kölcsönhatások, valamint külső szolgáltatások integrációjának tesztelésére összpontosít, és kihívásokkal járhat, mint például külső hibák kezelése.

- Elfogadási tesztelés (Acceptance Testing): 
  - A felhasználók által végzett tesztelés, amely azt ellenőrzi, hogy a rendszer megfelel-e az üzleti igényeknek.

##

#### ✅ Mi a különbség a verifikáció és a validáció között?

#### Verifikáció: 
- Az a folyamat, amely biztosítja, hogy a fejlesztett termék megfeleljen a tervezési specifikációknak és követelményeknek.

#### Validáció: 
- Az a folyamat, amely biztosítja, hogy a fejlesztett termék megfeleljen a felhasználói igényeknek és elvárásoknak.

##

#### ✅ Mik a tesztelési típusok, és mi a különbség köztük?

#### Funkcionális tesztelés: 
- A funkciók működését ellenőrzi, hogy a rendszer a specifikációnak megfelelően működik.

#### Nem-funkcionális tesztelés: 
- A rendszer teljesítményét, biztonságát, használhatóságát és más nem funkcionális tulajdonságait vizsgálja.

#### Fehér doboz tesztelés: 
- A tesztelő ismeri a kódot, és a belső működést ellenőrzi (pl. kódborítás).

#### Ellenőrző tesztelés tesztelés: 
- A tesztelő nem ismeri a kód belső struktúráját, és kizárólag a szoftver külső működését vizsgálja a bemenetek és kimenetek alapján.

#### Regressziós tesztelés: 
- A tesztelő részleges ismeretekkel rendelkezik a rendszer belső működéséről, és azokat az ismereteket felhasználva végzi el a tesztelést.

##

#### ✅ Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?

#### Fehér doboz tesztelés: 
- A tesztelő teljes hozzáféréssel rendelkezik a kódhoz és annak belső struktúrájához. A tesztelés célja a kód hibáinak megtalálása és az optimalizálás.

#### Szürke doboz tesztelés: 
- A tesztelő részleges hozzáféréssel rendelkezik a rendszer belső működéséhez. Különböző kód vagy konfigurációs információk alapján végezhet tesztelést.

#### Fekete doboz tesztelés: 
- A tesztelő nem ismeri a rendszer belső működését, csak a bemeneteket és kimeneteket vizsgálja.

##

#### ✅ Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?

#### UAT (User Acceptance Testing): 
- A végfelhasználók vagy az üzleti szereplők végzik, hogy biztosítsák, hogy a rendszer megfelel az üzleti követelményeknek. Ez a tesztelési fázis biztosítja, hogy a termék használható és elfogadható a felhasználók számára.

#### Rendszerteszt: 
- A rendszert mint egységet tesztelik, hogy az minden előírt specifikációnak megfeleljen, de nem feltétlenül foglalkozik az üzleti szempontokkal.

##

#### ✅ Sorolj fel különbségeket a regressziós tesztelés, a füsttesztelés és az újratesztelés között!

#### Regressziós tesztelés: 
- A szoftver frissítése vagy módosítása után végzik, hogy ellenőrizzék, hogy az új kód nem okozott-e hibát a rendszer korábban jól működő részein.

#### Füsttesztelés: 
- Az alapvető működés ellenőrzése, hogy a legfontosabb funkciók működnek-e egy új build után. Ez egy gyors, felületes teszt mely a stabilitást ellenőrzi.

#### Újratesztelés: 
- Az adott hibák javítása után annak biztosítása, hogy a hiba valóban megszűnt, és hogy a javítás nem hozott létre új problémát.

- Újratesztelés kizárólag a kijavított hibák tesztelésére vonatkozik, hogy biztosítsák a hibák valódi megoldását.

##

#### ✅ Mi a különbség a statikus és dinamikus tesztelés között?

#### Statikus tesztelés: 
- A kód futtatása nélkül végzik, és elsősorban kódelemzésen, dokumentációellenőrzésen és követelmény-ellenőrzésen alapul.

#### Dinamikus tesztelés: 
- A kód futtatásával történik, és a rendszer viselkedését teszteli a működés közben, hibák és anomáliák keresésével.

##

### ✅ Hasonlítsd össze a V-modellt, a vízesés modellt és az Agile megközelítést a tesztelés szempontjából!

V-modell: 
- A tesztelés a fejlesztési fázisokkal párhuzamosan halad. Minden egyes fejlesztési szakaszhoz kapcsolódik egy megfelelő tesztelési fázis. A tesztelés szisztematikusan, szigorúan követi a fejlesztést.

Vízesés modell:
- A fejlesztési fázisok lineárisan következnek egymás után. A tesztelés csak a fejlesztési fázis befejezése után történik.

Agile megközelítés: 
- A tesztelés folyamatos és iteratív folyamat, amely minden sprintben és iterációban jelen van, így gyorsabb és rugalmasabb a változások kezelésében.
##

<img src="https://t4.ftcdn.net/jpg/03/90/15/65/360_F_390156585_8w1lsOyICIAOvDCU8tExXW2QwLCOFwXD.jpg" alt="image" width="550" height="400">


<img src="https://i.imgur.com/S38EBJw.png" alt="image" width="550" height="400">   <img src="https://segedletek.level14.hu/assets/img/modszertan-vizeses.svg" alt="image" width="550" height="400">


<img src="https://promanconsulting.hu/wp-content/uploads/2022/03/agilis-modszertanok-optimized.jpg" width="550" height="400">

## Reporting, Bugs
<img src="https://moolya.com/blog/wp-content/uploads/2023/05/Bug-Report.png" alt="image" width="300" height="220">

#### ✅ Milyen lépéseket követnél egy hiba megtalálásakor?
- Hiba észlelése
  - A tesztelés során a teszteset eredményét összevetjük az elvárt eredménnyel. Ha eltérés tapasztalható, azt hibának tekintjük.
- Hiba dokumentálása (hibajegy létrehozása) ->
Rögzítjük a hibát egy hibakövető rendszerben.
  - Részletezzük:
    - milyen környezetben történt,
a hiba pontos leírása,
hogyan lehet reprodukálni,
képernyőképek, naplók, verziószám stb.
- Hiba elemzése és osztályozása
  - Megállapítjuk a hiba súlyosságát és prioritását.
Azonosítjuk, hogy melyik komponens vagy fejlesztő felelős.
- Hiba továbbítása fejlesztőknek
  - A hibát kijavításra továbbítjuk, megfelelő prioritással és minden szükséges információval.
- Hiba kijavítása és ellenőrzése (retesztelés):
  - A fejlesztő kijavítja a hibát.
A tesztelő újra lefuttatja a tesztesetet (ellenőrző teszt), hogy meggyőződjön a javítás sikerességéről.
- Regrssziós tesztelés
  - Ellenőrizzük, hogy a hiba javítása nem okozott új hibát más funkciókban.
- Hibajegy lezárása:
  - Ha a hiba javítása megerősítést nyer, a hibajegyet lezárják.

##

#### ✅ Beszélj a gyakori tesztjelentésekről és részleteikről!

#### Az elvégzett tesztelés összefoglalása:
- Tájékoztatás a tesztelési időszak alatt történtekről
- Eltérések a tervtől, beleértve a tesztelési tevékenységek ütemtervét, időtartamát vagy a ráfordításokat
- A tesztelés és a termékminőség állapota a kilépési kritériumok vagy a „kész” definíciójának
tekintetében
- Azok a tényezők, amelyek blokkolták vagy továbbra is blokkolják a haladást
- A hibák, a tesztesetek, a teszt lefedettség, a tevékenység előrehaladása és az erőforrás-fogyasztás
mérőszámai
- A fennmaradó kockázatok
- Újrahasznosítható tesztelési munkatermékek

##

#### ✅ Mit tartalmaz egy hibajelentés?

#### A dinamikus tesztelés során létrehozott hibajelentés általában a következőket tartalmazza:
- Azonosító
- A bejelentett hiba címe és rövid összefoglalása
- A hibajelentés dátuma, a kibocsátó szervezet és a szerző
- A tesztelem (az éppen tesztelt konfigurációs elem) és a környezet azonosítója
- A fejlesztési életciklus fázisa(i), amelyben a hibát észlelték
- A hiba reprodukálását és megoldását lehetővé tevő leírás, beleértve a naplófájlokat, az adatbázis-
mentéseket, képernyőképeket vagy felvételeket (ha volt ilyen a teszt végrehajtása során)
- Elvárt és tényleges eredmények
- A hiba súlyosságának (severity) hatóköre vagy mértéke az érdekelt felek érdekeit tekintve
- A javítás sürgőssége/prioritása
- A hibajelentés állapota (pl. nyitott, elhalasztott, duplikált, megoldásra váró, ellenőrző tesztelésre váró,
újranyitva, lezárt)
- Következtetések, ajánlások és jóváhagyások
- Globális problémák, például olyan területek, amelyekre a hibából eredő változás hatással lehet
- Változási előzmények, mint például a projektcsapat tagjai által a hibával kapcsolatos lépések, hogy
elkülönítsék, javítsák és ellenőrizzék azt
- Hivatkozások, beleértve a problémát feltáró tesztesetet is

##

#### ✅ Hogyan rangsorolnál egy hibát?
 - kritikus -> pl. rendszer összeomlik
 - magas -> pl. funkció hibásan működik
 - közepes -> pl. egy funkció nem működik, de nem minden felhasználót érint.
 - alacsony -> pl. kisebb esztétikai hiba

##


## Test Automation, Selenium
<img src="https://media.licdn.com/dms/image/C4D12AQE3GOyVsZazOw/article-cover_image-shrink_600_2000/0/1583830696602?e=2147483647&v=beta&t=bYHbKyhMoWsMgtEug6eSf3m0db5ZtGEl437TeS1qkfI" alt="image" width="320" height="220">

#### ✅ Melyik teszteseteket érdemes automatizálni és melyiket nem?

- #### Automatizálásra alkalmasak:
  - Gyakran ismétlődő tesztek (pl. regressziós tesztek)
  - Nagy adatállományon futó tesztek (pl. teljesítménytesztek)
  - Stabil, ritkán változó funkciók
  - Időigényes manuális tesztek
  - Több konfiguráción (pl. böngészőn) ismétlődő tesztek
  - Objektíven értékelhető eredményekkel rendelkező tesztek

- #### Általában nem érdemes automatizálni:
  - Egyszer lefutó vagy ritkán ismételt tesztek
  - Gyorsan változó felületű vagy logikájú funkciók
  - Nagyon komplex tesztek, amelyek automatizálása aránytalanul drága
  - Szubjektív értékelésű tesztek (pl. vizuális megjelenés, UX)
  - Felfedező tesztek

##

#### ✅ Írj le egy jó automatizált tesztet!

| Tulajdonság                  | Leírás |
| - | - |
| **Megbízható**               | A helyes eredményt adja minden futtatásnál, ha nem történt változás.    |
| **Karbantartható**           | Könnyen módosítható a rendszer változása esetén.                        |
| **Gyorsan fut**              | Nem fogja vissza a fejlesztési ciklust.                                 |
| **Önállóan futathazó**       | Nem függ más tesztektől – önállóan lefuttatható.                        |
| **Jól dokumentált**          | Érthető, mit tesztel és miért – neve, kommentek, szerkezet.             |
| **Hasznos visszajelzést ad** | Hibás működés esetén pontos hibaüzenetet ad, nem csak FALSE-t vagy FAIL-t.         |

##

#### ✅ Mi a Selenium, Selenium IDE és Selenium WebDriver?
- A Selenium webalkalmazások automatikus tesztelésére szolgáló keretrendszer. Ez széles körben használható eszköz és az egyik legismertebb nyílt forrású teszteszköz.
- A Selenium IDE egy nyílt forráskódú tesztautomatizálási eszköz, amely rögzítheti és lejátszhatja az interneten végzett műveleteit. Használatával automatizálhatja a webalkalmazások tesztelését.
- A Selenium WebDriver egy webes keretrendszer, amely lehetővé teszi a böngészők közötti tesztek végrehajtását. Ez az eszköz a webalapú alkalmazások tesztelésének automatizálására szolgál annak ellenőrzésére, hogy az elvárt módon működik-e. A Selenium WebDriver lehetővé teszi a programozási nyelv kiválasztását tesztszkriptek létrehozásához.

##

#### ✅ Hogyan lehet azonosítani a webes elemeket?

- 

##

#### ✅ Hogyan lehet várni az elemekre, és mi lehet a probléma? Gyűjtsd össze a lehetséges hibákat és okokat!



##

#### ✅ Hasonlítsd össze a POM és a Keyword Driven Testing megközelítéseket!

- A POM a felhasználói felület elemeivel való interakcióra összpontosít, míg a kulcsszóvezérelt tesztelés az alkalmazáson végzett magas szintű műveletekre összpontosít. Együtt használhatók a robusztusabb tesztelési megközelítés érdekében. 
- Bonyolultság és kódolás: A POM több kódolási képességet igényel, így összetettebb, de rugalmasabb.

##

#### ✅ Mi a különbség a TDD és BDD között?

- A TDD elsősorban az egységtesztekre és a kódfunkcionalitásra összpontosít, a BDD a rendszer viselkedésére és az érdekelt felekkel való együttműködésre összpontosít, az ATDD pedig elfogadási kritériumok révén összehangolja a fejlesztést a felhasználói követelményekkel.

##

#### ✅ Mi az API tesztelés és miért hasznos?

##

#### ✅ Mi az adatvezérelt tesztelés és miért hasznos?

##
[Solid Principles robot explanation](https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898/)