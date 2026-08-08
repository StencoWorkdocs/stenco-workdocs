# WorkDocsi arhitektuur

## 1. Üldpõhimõte

WorkDocs on moodulitest koosnev digitaalne tööhalduse süsteem.

Süsteemi eesmärk on koondada ettevõtte tööga seotud info ühte kohta ning anda igale kasutajale tema rollile vastav lihtne vaade.

WorkDocs peab olema:

- lihtne kasutada;
- loogiline;
- paindlik;
- laiendatav;
- turvaline;
- töökindel.

Süsteemi keerukus peab jääma kasutaja eest võimalikult palju taustale.

---

## 2. Üks süsteem, üks andmestik, erinevad vaated

WorkDocs kasutab ühist andmestikku.

Sama info ei tohiks olla erinevates kohtades korduvalt sisestatud.

Näiteks:

Töötaja sisestab oma töötunnid ühe korra.

Sama info on seejärel vajadusel nähtav:

- töötajale;
- objektijuhile;
- projektijuhile;
- kontorile;
- aruannetes.

Kasutaja näeb ainult talle lubatud infot.

> Sisesta üks kord. Kasuta mitmel pool.

---

## 3. Peamised süsteemikihid

WorkDocs koosneb põhimõtteliselt järgmistest kihtidest:

### Kasutajaliides

Kasutaja suhtleb WorkDocsiga veebipõhise kasutajaliidese kaudu.

Kasutajaliides peab töötama:

- arvutis;
- tahvelarvutis;
- telefonis.

Töötaja jaoks peab kasutamine olema eriti mugav mobiilseadmes.

---

### Rakendusloogika

Rakendusloogika juhib:

- kasutajate õigusi;
- töövooge;
- objektide infot;
- tööaja arvestust;
- materjale;
- lisatöid;
- dokumente;
- kinnitusi;
- teavitusi.

---

### Andmebaas

Andmebaasis säilitatakse WorkDocsi põhiinfo.

Näiteks:

- kasutajad;
- rollid;
- objektid;
- projektid;
- töötunnid;
- tööülesanded;
- materjalid;
- fotod;
- lisatööd;
- dokumendid;
- digitaalsed kinnitused;
- sõidukid;
- inventar;
- sündmuste ajalugu.

---

## 4. Moodulipõhine ülesehitus

WorkDocs ei pea kõiki funktsioone korraga sisaldama.

Süsteem peab olema ehitatud moodulitena.

### WorkDocs Core

Esimene põhiosa:

- kasutajad;
- rollid;
- objektid;
- tööajad;
- tööülesanded;
- päevaaruanded;
- teavitused.

### Projektide haldus

- objektide info;
- tööetapid;
- materjalid;
- fotod;
- dokumendid;
- projekti ajalugu.

### Tellija

- objekti ülevaade;
- lisatööde tellimine;
- kommentaarid;
- tööetappide kinnitamine;
- digitaalne allkirjastamine.

### Autode haldus

- sõidukite register;
- kasutajad;
- läbisõit;
- hooldused;
- ülevaatused;
- kindlustused;
- rikked;
- kasutusajalugu.

### Inventar

- tööriistad;
- seadmed;
- akud;
- masinad;
- vastutajad;
- asukoht;
- kasutusajalugu.

### Raportid

- töötunnid;
- objektide kokkuvõtted;
- materjalikulu;
- lisatööd;
- projektide ülevaated.

---

## 5. Kasutajaliidese põhimõte

Kasutaja ei pea nägema kogu WorkDocsi.

Pärast sisselogimist avaneb kasutajale tema rollile vastav vaade.

Näiteks töötaja näeb:

- Minu päev;
- Minu tööleht;
- Minu nädal;
- Tänased tööülesanded;
- Objektiga seotud info;
- Lisatööd;
- Vajadusel fotod ja materjalid.

Objektijuht näeb rohkem infot.

Kontor näeb ettevõtte tööaja ja aruandluse infot.

Tellija näeb ainult oma objektiga seotud infot.

---

## 6. Kodulehe ja WorkDocsi ühendus

WorkDocs peab olema võimalik siduda ettevõtte kodulehega.

Näiteks:

Stenco Gruppi koduleht
→ WorkDocs
→ Logi sisse

Pärast sisselogimist suunatakse kasutaja talle sobivasse WorkDocsi vaatesse.

WorkDocs võib olla kasutatav nii:

- ettevõtte kodulehe osana;
- eraldi veebirakendusena;
- mobiilse veebirakendusena.

---

## 7. Info liikumine

WorkDocsi üks tähtsamaid ülesandeid on info liikumine.

Näide:

Tellija lisab lisatööde soovi
↓
WorkDocs registreerib soovi
↓
Objektijuht näeb lisatööd
↓
Töötaja näeb talle vajalikku infot
↓
Töö tehakse
↓
Töötaja märgib töö tehtuks
↓
Vajadusel lisatakse foto
↓
Objektijuht kontrollib
↓
Tellija näeb valminud etappi
↓
Tellija kinnitab töö
↓
Kinnitus jääb projekti ajalukku.

---

## 8. Ajalugu ja jälgitavus

Oluline info peab jääma süsteemi ajalukku.

WorkDocs peab võimaldama hiljem tuvastada:

- kes info sisestas;
- millal info sisestati;
- mida muudeti;
- kes muudatuse tegi;
- millal töö kinnitati;
- millal tellija allkirjastas.

Eesmärk on, et projekti kohta oleks võimalik ka kuude või aastate pärast vajalik info üles leida.

---

## 9. Lihtsuse reegel

WorkDocsi kõige tähtsam arhitektuuriline põhimõte:

> Süsteem võib olla taustal keeruline, kuid kasutaja jaoks peab see olema lihtne.

Iga uue funktsiooni lisamisel tuleb küsida:

1. Kas see lahendab päris probleemi?
2. Kas see teeb kasutaja töö lihtsamaks?
3. Kas sama tulemust saab saavutada lihtsamalt?
4. Kas kasutaja peab selle kasutamiseks midagi uut õppima?

Kui funktsioon ei anna kasutajale piisavalt väärtust, ei lisata seda süsteemi.

---

## 10. Arhitektuuri areng

WorkDocs ehitatakse etapiviisiliselt.

Esimene eesmärk ei ole valmis ehitada kogu süsteemi.

Esimene eesmärk on luua töötav ja kasutatav põhiosa:

> Töötaja → tööaeg → objekt → info → kontor.

Seejärel lisatakse järk-järgult:

- päevaaruanded;
- materjalid;
- fotod;
- lisatööd;
- tellija;
- kinnitused;
- digitaalne allkirjastamine;
- dokumendid;
- autod;
- inventar;
- raportid.

Iga järgmine moodul peab toetama olemasolevat süsteemi, mitte muutma seda keerulisemaks.
