# swecalc

Svenska kalkylatorer för privatekonomi, investeringar och boende. Projektet innehåller bland annat ränta-på-ränta-beräkning, bostadslånekalkyl och en matvaruskanner som kan slå upp produkter via streckkod.

**Live:** https://todd3n.github.io/swecalc/

## Användning

Öppna livesidan i en modern webbläsare. Kalkylatorerna körs i webbläsaren och kräver ingen inloggning.

## Streckkodsskanning

Matvaruskannern använder kameran för att läsa produktens streckkod och söker sedan efter produkten i Open Food Facts.

- Ge webbläsaren tillåtelse att använda kameran.
- Använd HTTPS; moderna webbläsare kräver en säker kontext för kameraåtkomst (localhost fungerar också vid lokal utveckling).
- Rikta kameran mot produktens EAN/UPC-streckkod med god belysning.
- Om kameran inte fungerar kan streckkoden anges manuellt.
- Produktuppgifter beror på Open Food Facts databas och kan saknas eller vara ofullständiga.

Kamerastöd och behörighetsdialoger varierar mellan webbläsare och enheter.

## Begränsningar

Näringsvärden, allergeninformation och produktbilder kommer från externa produktposter. De ska inte betraktas som en garanti för innehållet i en vara. Läs alltid förpackningens aktuella ingrediens- och allergenmärkning, särskilt vid allergier eller överkänslighet.

## Lokal utveckling

Projektet är en statisk webbapp. Öppna `index.html` via en lokal utvecklingsserver eller publicera filerna på en HTTPS-kompatibel statisk webbhost. Undvik att öppna filen direkt via `file://` om du vill använda kameran.

## Externa tjänster

- [Open Food Facts](https://world.openfoodfacts.org/) – produkt- och näringsinformation
- [Chart.js](https://www.chartjs.org/) – diagram
- [html5-qrcode](https://github.com/mebjas/html5-qrcode) – kamerabaserad streckkodsläsning

## Licens

Ingen licens är angiven ännu. Kontakta repository-ägaren innan du återanvänder eller distribuerar koden.
