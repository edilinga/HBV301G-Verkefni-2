# Software Requirements Specification (útgáfa fyrir verkefni 2)

## Númer teymis og höfundar
* **Teymi:** Inga og Gabríel
* **Höfundar:** Edil Inga Kristjánsdóttir og Gabríel Orri Karlsson

## Heiti kerfis
**Vaktin** (Sveigjanlegt vaktaplan og afleysingakerfi fyrir veitingastaði og verslanir)

## 1. Inngangur

### 1.1 Gildissvið (Scope)
Vaktin er hugbúnaðarlausn sem auðveldar starfsfólki í vaktavinnu að óska eftir vaktaskiptum, finna afleysingar og framkvæma vaktaskipti með skjótum og öruggum hætti. Kerfið dregur úr yfirlegu vaktstjóra við handvirkar breytingar á vaktaplani og tryggir að allar breytingar séu í samræmi við vinnulöggjöf og kjarasamninga (t.d. lágmarkshvíldartíma). 

**Innan marka kerfisins (In-Scope):**
* Umsýsla og óskir um vaktaskipti milli starfsmanna í rauntíma.
* Sjálfvirk regluvörsla (viðvaranir vegna hvíldartíma og starfshæfni).
* Samþykktarferli stjórnenda og rauntímatilkynningar (push notifications).

**Utan marka kerfisins (Out-of-Scope):**
* Upphafleg gerð vaktaplans frá grunni og launaútreikningar (flutt inn/út í gegnum ytri skil).

### 1.2 Tilvísanir
* **IEEE 29148** staðall um kröfugerð í hugbúnaðarverkfræði (*Systems and software engineering — Life cycle processes — Requirements engineering*).
* **Karl Wiegers & Joy Beatty:** *Software Requirements (3rd Edition)* – COS Vision & Scope fyrirmynd.

## 2. Lýsing á hagsmunaaðilum og notendahópum

Helstu hagsmunaaðilar Vaktarinnar skiptast í beina notendur (starfsfólk og vaktstjórar) og óbeina notendur (launadeild og rekstraraðilar). Starfsfólk þarf skjótan og einfaldan aðgang í gegnum snjallsíma til að losna við eða taka að sér vaktir, á meðan vaktstjórar krefjast yfirsýnar og rekstraröryggis. Nákvæmari greiningu á hagsmunaaðilum, þörfum þeirra, notendahópum og persónu (Söru Jónsdóttur) má finna í sérstakri skrá:

[Hagsmunaaðilar og notendahópar](STAKEHOLDERS.md)

## 3. Greining á mögulegum árekstrum og tillögu að úrlausnum

Aðalársksturinn í kerfinu varðar kröfuna um **sjálfvirkni og hraða** hjá starfsfólki á móti kröfuna um **stýringu og rekstraröryggi** hjá vaktstjórum. Lausnin felst í *skilyrtri sjálfvirkni (Conditional Auto-Approval)* þar sem kerfið samþykkir vaktaskipti sjálfvirkt ef hæfni er sú sama og reglum er fylgt, en vísar flóknari tilvikum til handvirkrar samþykktar vaktstjóra. Nákvæma greiningu á árekstrinum og úrlausn hans má finna í:

[Árekstrar og úrlausnir](CONFLICTS.md)

## 4. Verkaskipting og ígrundun

Verkefninu var skipt jafnt á milli tveggja hópmeðlima þar sem unnið var úr greiningum á hagsmunaaðilum (`STAKEHOLDERS.md`), greiningu á árekstrum og úrlausnum þeirra (`CONFLICTS.md`), ásamt því að tengja þær við viðskiptakröfur, notendakröfur og virknikröfur kerfisins. Nánari samantekt um verkaskiptingu, endurmat og svör um hvað gekk vel og hvað mátti bæta eru dregin saman í skránni:

[Verkaskipting og ígrundun](Vinnuferli.md)

## 5. Vinnuferli

Vinnuflæði hópsins var framkvæmt með Git og GitHub. Vinnulag fólst í því að stofna Issue fyrir verkþætti, vinna á aðskildum greinum, vista breytingar með commit og push og senda síðan Pull Request (PR), þar sem hinn hópmeðlimurinn rýndi breytingarnar áður en þær voru sameinaðar við main greinina. Nánari lýsingu á vinnuferli, verkaskiptingu og ígrundun má finna í skránni:

[Vinnuferli](Vinnuferli.md)
