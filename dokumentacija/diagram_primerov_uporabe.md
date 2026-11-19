
# SpendWise – Diagram primerov uporabe

Diagram prikazuje ključne funkcionalnosti mobilne aplikacije SpendWise.

```mermaid
flowchart LR
    U["👤 Uporabnik"]

    subgraph S["Sistem SpendWise"]
        A([Registracija in prijava])
        B([Upravljanje transakcij])
        C([Mesečni proračun])
        D([Pregled statistike])
        E([Varčevalni cilji])
        F([Opozorila])
    end

    U --- A
    U --- B
    U --- C
    U --- D
    U --- E
    U --- F
```

## Opis

Uporabnik lahko:
- Ustvari račun in se prijavi.
- Dodaja, ureja in briše finančne transakcije.
- Nastavlja mesečne proračune.
- Pregleduje statistiko prihodkov in odhodkov.
- Upravlja varčevalne cilje.
- Prejema opozorila o porabi.
