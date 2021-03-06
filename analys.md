# Analys av data

Att analysera en skivavbildning kan ta mycket tid i anspråk om disken är stor, exempelvis kan den automatiska utläsningen av metadata från 10GB-disk i dagsläget ta flera timmar och extraktionen av alla filer på disken kan ta flera dagar.

## Extraktion av metadata

Efter att skivavbildningen är gjord kan bör man, för att få en överblick av innehållet på disken, göra en extraktion av så mycket metadata som möjligt.
Verktyg finns för att läsa ut denna metadata i olika former:

* **Statistisk form:**
antal filer, antal raderade filer, antal worddokument, antal pdf:er, antal bildfiler etc (BitCurator: *BitCurator Reporting Tool*)

* **XML-form (dfxml):**
hela filstrukturen kodas i xml med namn, positioner och checksummor på mappar och filer (BitCurator: *FiWalk*)

* **Mönstermatchning:**
resultat av sökningar på olika strängmönster som t ex epost-adresser, url:er, personnummer etc (BitCurator: *Bulk-extractor*)

## Bedömning av metadata
En hårddisk innehåller många
filer som inte är intressanta för vidare analys, exempelvis programvaru- eller operativsystemfiler. Majoriteten av filerna på en hårddisk utgörs oftast av den här typen.

En stor del av filerna går att sortera bort automatiskt, men det kommer ändå alltid att återstå en ganska stor mängd som är'potentiellt relevanta'

Framsortering av de intressanta filerna tillhör en av de mer tidskrävande delarna i analysen eftersom det i slutändan måste göras manuellt av en arkivarie.

>Med analysen som bakgrund kan man alltså välja vilka filer som kan vara intressanta att extrahera från skivavbildningen.













