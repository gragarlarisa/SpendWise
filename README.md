
# SpendWise 💜

## Aplikacija za upravljanje osebnih financ

SpendWise je mobilna aplikacija, namenjena preprostemu
spremljanju osebnih prihodkov, odhodkov, mesečnih
proračunov in varčevalnih ciljev.

Projekt nastaja v okviru predmeta
**Razvoj vseprisotnih informacijskih rešitev (RVIR)**
v študijskem letu 2026/2027.

## Glavne funkcionalnosti

- Registracija in prijava uporabnika.
- Dodajanje, urejanje in brisanje transakcij.
- Razvrščanje prihodkov in odhodkov po kategorijah.
- Nastavljanje mesečnih proračunov.
- Pregled statistike in grafov porabe.
- Ustvarjanje in spremljanje varčevalnih ciljev.
- Opozorila ob približevanju omejitvam porabe.

## Uporabljene tehnologije

| Tehnologija | Namen |
|---|---|
| Flutter | Razvoj mobilne aplikacije |
| Dart | Programski jezik |
| Supabase | Avtentikacija in zaledne storitve |
| PostgreSQL | Podatkovna baza |
| GitHub | Upravljanje izvorne kode |
| GitHub Actions | Avtomatizirano preverjanje kode |

## Arhitektura

Aplikacija je načrtovana s tremi logičnimi plastmi:

1. Predstavitvena plast – Flutter uporabniški vmesnik.
2. Poslovna logika – izračuni, validacija in proračuni.
3. Podatkovna plast – povezava s Supabase in PostgreSQL.

Podrobnosti so opisane v dokumentaciji projekta.

## Projektna dokumentacija

Dokumentacija se nahaja v mapi
[dokumentacija](dokumentacija/).

Vključuje:
- Projektno zasnovo in opis funkcionalnosti.
- Diagram primerov uporabe.
- Mockupe uporabniškega vmesnika.
- Začetni podatkovni model.
- Arhitekturo aplikacije.

## Zagon projekta

Za lokalni zagon je treba namestiti Flutter SDK.

```bash
git clone https://github.com/gragarlarisa/SpendWise.git
cd SpendWise
flutter pub get
flutter run
```

Za zagon v brskalniku Chrome:

```bash
flutter run -d chrome
```

## Testiranje in CI

Projekt uporablja GitHub Actions.

Ob spremembah na veji `main` se samodejno izvajajo:

```bash
flutter pub get
flutter analyze
flutter test
```

## Načrt razvoja

Razvoj je razdeljen na naslednje faze:

1. Načrtovanje in priprava dokumentacije.
2. Implementacija prijave in registracije.
3. Implementacija transakcij in proračunov.
4. Implementacija statistike, varčevalnih ciljev
   in opozoril.
5. Testiranje, izboljšave in zaključna predstavitev.

Razvojne naloge in njihove prioritete so
evidentirane v zavihku GitHub Issues.

## Trenutno stanje projekta

Projekt je v začetni razvojni fazi.

Flutter aplikacija je ustvarjena in uspešno zagnana.
Pripravljena je začetna projektna dokumentacija,
vzpostavljeno je avtomatizirano preverjanje kode.

Poslovne funkcionalnosti in povezava s Supabase
bodo implementirane v naslednjih fazah.

## Avtorstvo

**Larisa Gragar**

Predvidena samostojna izvedba projekta.

Predmet: Razvoj vseprisotnih informacijskih rešitev
Študijsko leto: 2026/2027
