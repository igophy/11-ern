# 11-ern

Registrering av poeng i kortspillet 11-ern.

## Om appen

En selvinneholdt HTML-app (ingen avhengigheter, ingen byggsteg) for å registrere poeng og følge nivåprogresjonen i kortspillet 11-ern. Kan installeres som PWA på mobil og fungerer offline.

## Funksjonalitet

- **Spilleroppsett** — velg antall spillere (2–8) og skriv inn navn
- **Runderegistrering** — legg inn poeng per spiller; spillere sorteres automatisk fra laveste til høyeste totalpoeng med rangbadge (1., 2., 3.)
- **Nivåsystem** — 11 nivåer med stigende vanskelighetsgrad; huk av «Klarte nivået» for å rykke opp
- **Nivåoversikt** — viser alle spilleres nåværende nivå sortert fra høyeste til laveste
- **Vinnerskjerm** — vises automatisk når en spiller fullfører alle 11 nivåer
- **Rundehistorikk** — kollapsbart panel med alle registrerte runder; vis hvem som klarte nivået per runde
- **Rediger / slett runde** — korriger eller fjern en tidligere runde; nivåer beregnes automatisk på nytt
- **Spillhistorikk** — avsluttede spill lagres og vises med statistikk (seire, snittpoeng) på oppstartsskjermen
- **Mørkt tema** — følger systeminnstillingen automatisk; kan overstyres med 🌙/☀️-knapp
- **Oppdateringsvarsel** — banner vises automatisk når ny versjon er tilgjengelig
- **PWA** — installerbar på mobil, fungerer offline
- **Persistering** — tilstand lagres i `localStorage`

## Nivåer

| Nivå | Oppgave | Maks trumf |
|------|---------|-----------|
| 1 | Serie på 4 | 0 |
| 2 | Tress 2 ganger | 1 |
| 3 | Serie på 4 + tress | 1 |
| 4 | Serie på 5 | 2 |
| 5 | Tress 3 ganger | 2 |
| 6 | Serie på 5 + tress | 2 |
| 7 | Serie på 7 | 2 |
| 8 | Serie på 6 + tress | 3 |
| 9 | Serie på 4, 2 ganger | 2 |
| 10 | 5 like 2 ganger | 4 |
| 11 | Serie på 9 | 4 |

## Versjonshistorikk

| Versjon | Endring |
|---------|---------|
| v1.0.0 | Grunnleggende poengregistrering med oppsett, rundevisning og stillingside |
| v1.1.0 | Nivåsystem med 11 nivåer og «Klarte nivået»-avkrysning |
| v1.2.0 | Stillingssiden fjernet; spillere sortert etter poengsum i rundebildet |
| v1.3.0 | Rundehistorikk-panel og redigering av tidligere runder |
| v1.4.0 | PWA-støtte: manifest, service worker og offline-caching |
| v1.5.0 | Rangering i rundebildet, slett runde og vinnerskjerm |
| v1.6.0 | Automatisk oppdateringsvarsel ved ny versjon |
| v2.0.0 | Spillhistorikk og statistikk per spiller |
| v2.1.0 | Mørkt tema med automatisk systemdeteksjon og manuell toggle |
| v2.2.0 | Fjernet nivå fra poengoversikten, tydeligere totalpoeng og poenginndata |
| v2.3.0 | Klikkbare spilldetaljer i historikk, deaktiverte dobbelttrykk-zoom |

## Bruk

Åpne `index.html` i en nettleser, eller installer appen via «Legg til på hjemskjerm» i mobilnettleseren.
