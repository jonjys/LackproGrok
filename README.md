# LackProGrok — Karma Läcksök Pro v9.0 ULTIMATE

Enkel-fil-app för analys av Kamstrup flowIQ® 2200 akustisk läckagedetektering (ALD).

## Live

Efter Vercel-deploy: `https://lackprogrok.vercel.app` (eller din custom domain).

## Funktioner
- Drag & drop av "Filtrerade mätare"-Excel från READy/Kamstrup
- Smart klassificering: AKTIV / BEVAKA / MISSTÄNKT / VÄRMEPUMP / TILLFÄLLIGT / LAGAD / STÖRNING
- Bugfixar från v8.1:
  - Stats och tabell syns direkt efter analys (inga 0-tal tills klick)
  - Graf visar alla historikpunkter som default
  - E ≥ 40 dB kan aldrig klassas som "Stabil bakgrund"
- Klickbara stats-rutor, filter-chips, sök, Leaflet-karta, Chart.js-grafer
- Kopieringsknapp på adress, memo, stjärnor, XLSX-export
- Datumintervall-slider som Kamstrup-portalen

## Användning
1. Öppna appen (Vercel eller lokalt `index.html`)
2. Släpp 1–n Excel-filer (idag + tidigare veckor + äldre för 3-årshistorik)
3. Analys sker automatiskt
4. Filtrera, granska grafer, exportera

## Deploy till Vercel
1. Gå till [vercel.com/new](https://vercel.com/new)
2. Importera `jonjys/LackproGrok`
3. Deploy (ingen build behövs – ren static HTML)
4. (Valfritt) Sätt domain till `lackprogrok.vercel.app`

## Stack
- En enda `index.html`
- SheetJS (XLSX), Chart.js, Leaflet
- 100 % client-side, ingen backend
