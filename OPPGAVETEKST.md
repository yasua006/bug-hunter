# Snake


## Bestilling

Du har tatt over et Snake spill og tillhørende highscore server. Koden kjører, for det meste, men den er full av både kritiske og mindre alvorlige bugs. Du skal spille rollen som både tester og utvikler for å finne *og* fikse koden.

- **Tester:** Kjør programmet, let etter bugs, og rapporter dem som et GitHub issue.
- **Utvikler:** Fiks de raporterte feilene, og steng issues etterhvert som de er løst.

Bytt rolle hver gang du har funnet alle bugs du klarer eller har fikset alle raporterte feil.

---

## Oppsett
*Alle filer utenom OPPGAVETEKST.md er en del av prosjektet.*

1. **Fork eller clone** dette repoet til din GitHub bruker: [bug-hunter](https://github.com/ensva002/Bug-hunter/tree/main)  

2. Sett opp virituelt miljø i rot-mappen til prosjektet og installer dependencies
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   ```
3. Start serveren i et terminal vindu:
   ```bash
   python highscore_server/server.py
   ```
4. Start spillet i et annet terminal vindu:
   ```bash
   python snake_game/snake.py
   ```

OBS: husk å aktivere *venv* i begge vinduene

Om noe ikke fungerer med en gang, og du har satt opp prosjektet rett, så har du nok allerede støtt på din første bug, lag en rapport.

---

##  Tester

Din jobb i denne rollen er å finne bugs, du skal **ikke** fikse noe nå.

Spill spillet og test serveren. Bruk RapidAPI, `curl` eller browseren til å teste API-et.

### Ting å se etter

- Ting som kræsejr.
- Ting som ikke oppfører seg som forventet i forrhold til README.md
- *Edge cases*, prøv å gjør ting som utvikleren ikke forventer at en spiller ville gjort.
- Ting som mangler

### Raportert bugs

Rapporter feilene du finner med en gang du finner dem som et issue.

Dette er en øvelse i å skrive gode raporter, bruk malen, les materialet om testing i OneNote, og se på issues på større GitHub prosjekter.

Prøv å raporter en håndfull med bugs før du bytter til utvikler rollen.

---

## Utvikler

I rollen som utvikler skal du kun fikse de rapporterte feilene, finner du en ny bug i koden når du jobber, la den stå, å se om du kan finne den igjen som tester.

1. Gjør endringer i koden
2. Sjekk at bug-en faktisk er fikset
3. Commit med en beskrivende commit-melding:
   ```
   Fikset at man ikke kan gå gjennom veggen
   ```
4. Steng issues
Gå til issues, steng issuet til bug-en du fikset med en kommentar.

Tips, om commit meldingen starter med Fix #[issue nummer] så stenges automatisk issuet. Eksempel:
```
Fix #4: Fikset at man ikke kan gå gjennom veggen
```

Fiks så mange bugs du klarer før du går tilbake til *tester*-rollen

---

## Innlevering
Du leverer inn link til repoet på teams. pass på at det er public eller at du har gitt tilgang til din lærer (A: Endre - B: Torbjørn). Det regnes som ikke levert om vi ikke kan se det.

Det skal ikke brukes AI i denne oppgaven, sitter du fast kan du se på noen hint her: [bug-hunt-hjelp](https://ensva002.github.io/bug-hunt-hjelp/)
