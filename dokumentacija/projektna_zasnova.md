# SpendWise – Projektna zasnova

**Predmet:** Razvoj vseprisotnih informacijskih rešitev (RVIR)  
**Študijsko leto:** 2026/2027  
**Izvajalka:** Larisa Gragar  
**Način izvedbe:** Predvidoma samostojno

## 1. Opis projekta

SpendWise je mobilna aplikacija za upravljanje osebnih financ. Namenjena je uporabnikom, ki želijo spremljati svoje prihodke, odhodke, mesečne proračune in varčevalne cilje.

Aplikacija rešuje problem nepregledne osebne porabe, saj uporabnikom omogoča centralizirano beleženje finančnih transakcij in grafični prikaz njihove porabe.

Ciljna skupina so predvsem študenti, mladi zaposleni in drugi posamezniki, ki želijo izboljšati nadzor nad osebnimi financami.

## 2. Glavne funkcionalnosti

### 2.1 Registracija in prijava

Uporabnik lahko ustvari račun z elektronskim naslovom in geslom, se prijavi ter odjavi. Podatki posameznega uporabnika so ločeni od podatkov drugih uporabnikov.

### 2.2 Upravljanje prihodkov in odhodkov

Uporabnik lahko dodaja, ureja in briše transakcije. Vsaka transakcija vsebuje znesek, datum, vrsto, kategorijo in neobvezni opis.

### 2.3 Mesečni proračun

Uporabnik lahko določi mesečno omejitev porabe za posamezno kategorijo. Aplikacija izračuna porabljeni in preostali znesek.

### 2.4 Statistika in analitika

Aplikacija omogoča pregled prihodkov, odhodkov in finančnega stanja. Podatki so prikazani z grafi po kategorijah in časovnih obdobjih.

### 2.5 Varčevalni cilji

Uporabnik lahko ustvari varčevalni cilj, določi ciljni znesek in spremlja napredek varčevanja.

### 2.6 Opozorila

Aplikacija uporabnika opozori, ko poraba doseže določen delež proračuna ali preseže nastavljeno omejitev.

## 3. Ključni uporabniški scenariji

**Scenarij 1 – Dodajanje odhodka**

1. Uporabnik se prijavi.
2. Izbere možnost dodajanja transakcije.
3. Vnese znesek, kategorijo in datum.
4. Shrani transakcijo.
5. Aplikacija posodobi stanje in statistiko porabe.

**Scenarij 2 – Nastavitev mesečnega proračuna**

1. Uporabnik odpre razdelek Proračun.
2. Izbere kategorijo.
3. Določi mesečno omejitev.
4. Aplikacija spremlja porabo in izračunava preostanek.

**Scenarij 3 – Ustvarjanje varčevalnega cilja**

1. Uporabnik odpre razdelek Varčevanje.
2. Ustvari nov cilj.
3. Določi ime in ciljni znesek.
4. Beleži prihranke.
5. Spremlja napredek doseganja cilja.

## 4. Predvidene tehnologije

| Tehnologija | Namen |
|---|---|
| Flutter | Razvoj mobilne aplikacije |
| Dart | Programski jezik |
| Supabase | Avtentikacija in spletne storitve |
| PostgreSQL | Podatkovna baza |
| GitHub | Verzijsko upravljanje kode |
| GitHub Actions | Samodejno preverjanje kode in testiranje |
| Figma | Načrtovanje uporabniškega vmesnika |

## 5. Predvidena arhitektura

Aplikacija bo razdeljena na predstavitveno, poslovno in podatkovno plast.

- **Predstavitvena plast:** Flutter zasloni in uporabniški vmesnik.
- **Poslovna plast:** Validacija podatkov, izračuni stanja, proračunov in varčevalnih ciljev.
- **Podatkovna plast:** Dostop do podatkov prek Supabase API-ja in podatkovne baze PostgreSQL.

Za dostop do podatkov bodo uporabljena pravila Row Level Security (RLS), ki bodo omejevala dostop uporabnikov do njihovih lastnih zapisov.

## 6. Predvideni podatkovni model

Osnovne podatkovne entitete:

- **Uporabnik:** ID, elektronski naslov.
- **Kategorija:** ID, naziv, vrsta kategorije, uporabnik.
- **Transakcija:** ID, uporabnik, kategorija, znesek, datum, vrsta, opis.
- **Proračun:** ID, uporabnik, kategorija, mesec, leto, omejitev.
- **Varčevalni cilj:** ID, uporabnik, naziv, ciljni znesek, privarčevani znesek.

Med entitetami bodo vzpostavljene povezave s tujimi ključi. Posamezen uporabnik ima lahko več transakcij, proračunov in varčevalnih ciljev.

## 7. Načrt razvoja

**Faza 1:** Priprava projektne zasnove, diagramov in mockupov.

**Faza 2:** Vzpostavitev podatkovne baze, avtentikacije in osnovne navigacije.

**Faza 3:** Implementacija transakcij, proračunov in statistike.

**Faza 4:** Implementacija varčevalnih ciljev in opozoril.

**Faza 5:** Testiranje, izboljšave, dokumentacija in priprava predstavitve.

## 8. Organizacija dela

Projekt bo predvidoma izveden samostojno. Izvajalka bo odgovorna za načrtovanje, implementacijo, testiranje, dokumentacijo in predstavitev aplikacije.

Razvojne naloge bodo organizirane z GitHub Issues, spremembe kode pa bodo sledljive prek Git commitov in Pull Requestov.
