# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

## A tesztelés alapjai:
#### Mi a tesztelés célja? Mi nem az?
A megrendelő számára használhatóvá tenni a programot, nem tökéletessé
#### Mi a kapcsolat a tesztelés és a hibamegelőzés között?
Mind a kettőt a folyamat legelején kell elvégezni, nem kihagyható egyik sem.
#### Miért fontos, hogy a tesztelők függetlenek legyenek a fejlesztőktől?
Más szemszögből látják, nem ismerik a kódot, igy nem tudják, hogy pontosan mi, hol mit fogad el, hogy működik
#### Mi a veszélye annak, ha a fejlesztő maga teszteli a saját kódját?
Ugyan azzal teszteli, tudja mit hogyan kell csinálni, nem reális felhasználó
#### Mik a tesztelési alapelvek?
1. Teszt, teszt, teszt, kimerítő tesztelés nem lehetséges
2. Hibafürt
3. Növényvédő szer-paradoxon
4. A tesztelés bizonyítja, hogy a szoftverben vannak hibák
5. Hiba hiánya
6. Korai teszt a szoftverfolyamatban
7. A tesztelés kontextustól függ
(Igen kimásoltam)
#### Mit jelent az „alapvető tesztelési elv”, hogy „a kimerítő tesztelés lehetetlen”?
Egy egyszerű programnak is végtelensok tesztelése lehet. Nem hatékony és nem kivitelezhető
#### Mit jelent az „alapvető tesztelési elv”, hogy „a hibák halmozódnak”?
Hibák 80%-a a modulok 20%-ban találhatók általában. Nem szétoszlanak
#### Mit jelent az „alapvető tesztelési elv”, hogy „a tesztelés a kontextustól függ”?
Egy weboldalt, webshopot, asztali alkalmazást, mobilalkalmazást, szervert nem azonos módszerekkel tudunk tesztelni. Mindnek megvannak a sajátos eszközei.

## 2. Tesztelés a szoftverfejlesztés életciklusán át
#### Mik a tesztszintek, és mi a különbség köztük?
● Komponenstesztelés (más néven egységtesztelés): az egyes komponensek elkülönítve történő 
tesztelésére összpontosít. Gyakran speciális támogatást igényel, például teszttámogató 
szoftverkörnyezetet vagy egységteszt-keretrendszert. A komponenstesztelést általában a fejlesztők 
végzik a saját fejlesztési környezetükben.
● Komponensintegrációs tesztelés (más néven egységintegrációs tesztelés): a komponensek közötti 
interfészek és interakciók tesztelésére összpontosít. Erősen függ az integrációs stratégia 
megközelítésétől, mint a lentről-fölfelé, föntről-lefelé vagy nagy-bumm.
● Rendszertesztelés: a teljes rendszer vagy termék viselkedésére és képességeire összpontosít, 
gyakran magában foglalva a végponttól végpontig tartó feladatok funkcionális tesztelését és a 
minőségjellemzők nemfunkcionális tesztelését. Néhány nemfunkcionális minőségjellemző esetében 
előnyösebb teljes rendszeren, egy reprezentatív tesztkörnyezetben tesztelni (például 
felhasználhatóság esetében). Alrendszerek szimulációjának használata is lehetséges. A rendszer 
tesztelését független tesztcsoport is végezheti, és a rendszer specifikációihoz kapcsolódik.
● Rendszerintegrációs tesztelés: a tesztelt rendszer, egyéb rendszerek és külső szolgáltatások 
interfészeinek tesztelésére összpontosít. A rendszerintegrációs tesztelés megfelelő 
tesztkörnyezeteket kíván meg, lehetőleg minél hasonlóbbat az üzemeltetési környezethez.
● Elfogadási tesztelés: validálásra és a kiadásra való felkészültség demonstrálására összpontosít, 
más szavakkal, azt vizsgáljuk, hogy a rendszer valóban kielégíti-e a felhasználó üzleti igényeit. Ideális 
esetben az elfogadási tesztelést a tervezett felhasználók végzik. Fő formái: felhasználói elfogadási 
tesztelés (angolul user acceptance testing, UAT), működési elfogadási tesztelés, szerződéses és 
szabályozói elfogadási tesztelés, alfatesztelés és bétatesztelés.
A tesztszintek megkülönböztethetőek a következő, nem kimerítő paraméterek alapján, hogy elkerülhető 
legyen a teszttevékenységek átfedése:
● Teszt tárgya
● Tesztcélok
● Tesztbázis
● Hibák és meghibásodások
● Megközelítés és felelősségek

ISTQB-CTFL-Syllabus 2.2.1

#### Miért nem érdemes mindig ugyanazokat a teszteseteket futtatni (regressziós torzítás)?
Mert azok a hibák ki lesznek küszöbölve, de a többi nem.
#### Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
● Komponenstesztelés (más néven egységtesztelés): az egyes komponensek elkülönítve történő 
tesztelésére összpontosít. Gyakran speciális támogatást igényel, például teszttámogató 
szoftverkörnyezetet vagy egységteszt-keretrendszert. A komponenstesztelést általában a fejlesztők 
végzik a saját fejlesztési környezetükben.

#### Mi a különbség a verifikáció és a validáció között?
Egy másik gyakori félreértés a teszteléssel kapcsolatban, hogy teljes mértékben a teszt tárgyának 
verifikációjára fókuszál. A tesztelés valóban kiterjed a verifikációra, azaz a meghatározott követelményeknek 
való megfelelés ellenőrzésére, azonban tartalmazza a validációt is, amely azt ellenőrzi, hogy a rendszer 
megfelel-e a felhasználói, illetve más érdekelt felek igényeinek a működési környezetben. 
#### Mik a tesztelési típusok, és mi a különbség köztük?

2.2.2 Teszttípusok
Számos teszttípus létezik és alkalmazható egy projektben. Ebben a tantervben a következő négy teszttípust 
említjük meg:
Funkcionális tesztelés során a komponens vagy rendszer működését vizsgáljuk, abból a szempontból, 
hogy elvégzi-e a meghatározott funkcióit. A meghatározott funkciók azt fejezik ki, hogy „mit” kell tudnia a 
rendszernek elvégeznie. A fő céljai a funkcionális tesztelésnek: a funkcionális teljesség, a funkcionális 
helyesség és a funkcionális megfelelőség ellenőrzése.
Nemfunkcionális tesztelés során olyan tulajdonságokat ellenőrzünk, amelyek nem a komponens vagy 
rendszer funkcionális jellemzői. A nemfunkcionális tesztelés azt vizsgálja, hogy „miként" viselkedik a 
rendszer. A fő célja a nemfunkcionális szoftver-minőségjellemzők ellenőrzése. Az ISO/IEC 25010 szabvány 
a következő osztályozást adja a nemfunkcionális szoftver-minőségjellemzőknek:
● Teljesítményhatékonyság
● Kompatibilitás
● Használhatóság
● Megbízhatóság
● Biztonság
● Karbantarthatóság
● Hordozhatóság
Előfordulhat, hogy a nemfunkcionális tesztelés az életciklus korai szakaszában kezdődik (például a 
felülvizsgálatok, a komponenstesztelés vagy a rendszertesztelés részeként). Számos nemfunkcionális teszt 
származtatható funkcionális tesztekből, mivel egy már létező funkcionális teszt futtatása során 
ellenőrizhetünk nemfunkcionális jellemzőket is (például ellenőrizhetjük, hogy egy funkció végrehajtásához 
szükséges idő megfelelő-e, vagy végrehajtódik-e egy eltérő keretrendszeren belül). A későn megtalált 
nemfunkcionális hibák nagyban befolyásolhatják egy projekt sikerét. Nemfunkcionális tesztelés esetén néha 
szükségünk lehet specifikus tesztkörnyezetre, mint például használhatósági teszt esetén egy 
használhatósági laborra.
Certified Tester
Alapszintű tanúsítvány - Hivatalos magyar nyelvű tanterv
ISTQB® CTFL Version V4.0.1 – Magyar nyelvű tanterv 29/72 2024.03.01
© 2024 Magyar Szoftvertesztelői Tanács Egyesület
A feketedoboz tesztelés (lásd a 4.2. fejezetet) egy specifikációalapú teszttípus, ahol a tesztelés tárgyától 
különálló dokumentációkból származtatjuk a teszteseteket. A feketedoboz tesztelés fő célja a rendszer 
viselkedésének ellenőrzése a rendszer specifikációinak szempontjából.
A fehérdoboz tesztelés (lásd a 4.3. fejezetet) egy struktúraalapú teszttípus, ahol a rendszer belső 
szerkezete vagy az implementációja (például: kód, architektúra, munkafolyamat, adatfolyam) alapján 
származtatjuk a teszteseteket. A fehérdoboz tesztelés fő célja, hogy tesztekkel elfogadható szinten lefedjük 
a rendszer alapvető struktúráját.
Mind a négy teszttípus alkalmazható minden tesztszinten, bár a fókusz minden szinten más lesz. Számos 
különböző teszttechnika használható a tesztfeltételek és tesztesetek származtatására minden teszttípus 
esetében.

#### Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?

A feketedoboz tesztelés (lásd a 4.2. fejezetet) egy specifikációalapú teszttípus, ahol a tesztelés tárgyától 
különálló dokumentációkból származtatjuk a teszteseteket. A feketedoboz tesztelés fő célja a rendszer 
viselkedésének ellenőrzése a rendszer specifikációinak szempontjából.
A fehérdoboz tesztelés (lásd a 4.3. fejezetet) egy struktúraalapú teszttípus, ahol a rendszer belső 
szerkezete vagy az implementációja (például: kód, architektúra, munkafolyamat, adatfolyam) alapján 
származtatjuk a teszteseteket. A fehérdoboz tesztelés fő célja, hogy tesztekkel elfogadható szinten lefedjük 
a rendszer alapvető struktúráját.

szürkedoboz tesztelés: Kettő keveréke.

#### Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
● Rendszerintegrációs tesztelés: a tesztelt rendszer, egyéb rendszerek és külső szolgáltatások 
interfészeinek tesztelésére összpontosít. A rendszerintegrációs tesztelés megfelelő 
tesztkörnyezeteket kíván meg, lehetőleg minél hasonlóbbat az üzemeltetési környezethez.
● Elfogadási tesztelés: validálásra és a kiadásra való felkészültség demonstrálására összpontosít, 
más szavakkal, azt vizsgáljuk, hogy a rendszer valóban kielégíti-e a felhasználó üzleti igényeit. Ideális 
esetben az elfogadási tesztelést a tervezett felhasználók végzik. Fő formái: felhasználói elfogadási 
tesztelés (angolul user acceptance testing, UAT), működési elfogadási tesztelés, szerződéses és 
szabályozói elfogadási tesztelés, alfatesztelés és bétatesztelés.

#### Mi a különbség a statikus és dinamikus tesztelés között?
3.1.3 Statikus és dinamikus tesztelés közötti különbségek
A statikus és a dinamikus tesztelés kiegészíti egymást. Hasonló céljaik vannak, mert mindkettő támogatja a
hibák kimutatását a munkatermékekben (lásd az 1.1.1. fejezetet), de eltérések is vannak közöttük, mint 
például: 
● A statikus és a dinamikus tesztelés (a meghibásodások elemzésével) egyaránt a hibák megtalálására 
vezet, azonban van néhány hibatípus, amelyet csak statikus vagy dinamikus teszteléssel lehet 
megtalálni. 
● A statikus tesztelés közvetlenül a hibákat találja meg, míg a dinamikus tesztelés meghibásodásokat 
tár fel, amelyekből a csatolt hibák az ezt követő elemzés során határozhatók meg.
● A statikus tesztelés könnyebben kimutathat olyan hibákat, amelyek elhelyezkedése a kódban a 
ritkábban bejárt végrehajtási útvonalakon találhatók, vagy olyanokat, amelyek nehezen érhetők el 
dinamikus teszteléssel.
● Statikus tesztelés alkalmazható végre nem hajtható munkatermékek esetén, míg dinamikus tesztelés 
csak futtatható munkatermékek esetén alkalmazható.
● Statikus tesztelés felhasználható azon minőségjellemzők mérésére, amelyek a futtatható kódtól 
függetlenek (mint például karbantarthatóság), míg a dinamikus tesztelés felhasználható olyan 
minőségjellemzők mérésére, amelyek a kód végrehajtástól függenek (mint például a 
teljesítményhatékonyság).
A statikus tesztelés során könnyebben, és/vagy kevesebb ráfordítással megtalálható tipikus hibák közé 
tartoznak az alábbiak:
● Követelmény hibák (mint például inkonzisztenciák, kétértelműségek, ellentmondások, kihagyások, 
pontatlanságok, duplikációk)
● Tervezési hibák (mint például nem kellően hatékony adatbázis szerkezetek, szegényes 
modularizáció)
● Bizonyos típusú kódolási hibák (mint például meghatározatlan értékeket tartalmazó változók, létre 
nem hozott változók, elérhetetlen vagy duplikált kód, felesleges kód komplexitás)
● Eltérések a szabványoktól (mint például az elnevezési konvenciók be nem tartása a kódolási 
szabványoknál)
● Helytelen interfész specifikációk (mint például nem illeszkedő paraméter szám, típus, vagy sorrend)
● A biztonsági sebezhetőségek bizonyos típusai (mint például a puffer túlcsordulás)
● Hiányok vagy pontatlanságok a tesztbázis lefedettségben (mint például hiányzó tesztek egy adott 
elfogadási feltételre)

### Szoftverfejlesztési és tesztelési modellek(vízesés, V-modell, agilis modell):

A szoftverfejlesztési életciklusmodell (SDLC) egy absztrakt, magasszintű reprezentációja a
szoftverfejlesztési folyamatnak. A szoftverfejlesztési életciklusmodell definiálja, hogy a különböző fejlesztési
fázisok és egyéb, a folyamat során végrehajtott tevékenységek hogyan kapcsolódnak egymáshoz logikailag
és kronológiailag. Példák a szoftverfejlesztési életciklusmodellekre: szekvenciális fejlesztési modellek (pl.:
vízesés modell, V-modell), iteratív fejlesztési modellek (pl.: spirális modell, prototípus fejlesztés) és
inkrementális fejlesztési modellek (pl.: Unified Process).
<br>
<img src="https://testsigma.com/blog/wp-content/uploads/image-132.png" alt="image" width="500" height="auto"><br>
<img src="https://media.geeksforgeeks.org/wp-content/uploads/20231030123258/software-Testing-SDLC-V-model.webp" alt="image" width="500" height="auto"><br>
<img src="https://miro.medium.com/1*PDzFYucgvC4z668ncU2YLA.png" alt="image" width="500" height="auto">


### TDD, BDD modell jellemzői.

Néhány tevékenység a szoftverfejlesztési folyamatokon belül leírható részletesebb szoftverfejlesztési
módszerekkel és agilis gyakorlatokkal is. Például: elfogadásiteszt-vezérelt fejlesztés (angol irodalomban
ATDD), viselkedésvezérelt fejlesztés (BDD), szakterület-vezérelt tervezés (DDD), extrém programozás (XP),
feature-vezérelt fejlesztés (FDD), Kanban, Lean IT, Scrum és tesztvezérelt fejlesztés (TDD).

A TDD, ATDD és BDD hasonló fejlesztési megközelítések, ahol a tesztek meghatározása a fejlesztés
irányításának eszközeként szolgál. Mindegyik megközelítés megvalósítja a korai tesztelés elvét (lásd a 1.3.
fejezetet) és követi a shift left megközelítést (lásd: 2.1.5-ös fejezet), mivel a tesztek meghatározása előbb
történik, mint a kód megírásra. Ezek a megközelítések az iteratív fejlesztési modellt támogatják és az
alábbiak szerint lehet jellemezni őket:
Tesztvezérelt fejlesztés (TDD):
● A kódolást tesztesetek irányítják (az átfogó szoftvertervek helyett) (Beck 2003)
● Először a tesztek kerülnek megírásra, majd azt követően a kód, olyan módon, hogy a teszteknek
megfeleljen. Végül a teszteket és a kódot is refaktorálják.
Elfogadásiteszt-vezérelt fejlesztés (ATDD) (lásd a 4.5.3. fejezetet):
● A teszteket elfogadási feltételekből származtatja a rendszertervezési folyamat részeként (Gärtner
2011)
● A teszteket az előtt írják meg, hogy lefejesztésre kerülne az alkalmazás azon része, mely kielégíti
ezeket a teszteket.
Viselkedésvezérelt fejlesztés (BDD)
● Kifejezi az alkalmazás kívánt viselkedését olyan tesztesetekkel, melyek egyszerű formában,
természetes nyelven vannak megírva, és így könnyen érthető az érdekelt felek számára – általában
a "Given/When/Then" formát használva (Chelimsky 2010)
● A teszteseteket ezután automatikusan végrehajtható tesztekké alakítják.
A fent említett megközelítések alkalmazása során, a tesztek megmaradhatnak automatizált tesztek
formájában, hogy biztosítsák a kód minőségét jövőbeli módosítások esetén.
