# Lagring av data
Digitala filer såsom dokument, skivavbildningar samt dess metadata, som har en anknytning till ett personarkiv eller liknande bör lagras med fullvärdig integritet gällande backuprutiner och dylikt.

## Lagring av skivavbildningar
Då skivavbildningar lagras, är det viktigt att ta hänsyn till den metadata som producerats utifrån skivavbildningen, vanligtvis i form av *DFXML*, som är ett standardformat för att dokumentera skivavbildningar samt dess innehåll.

Då informationen i en skivavbildningfils DFXML innehåller information om filer, filsystem, filstorlek, ändrad-datum, raderade filer et c, är det relevant information att spara på ett säkert vis, oavsett ifall skivavbildningen lagras eller ej.

DFXML ger möjlighet att referera extraherade filer till en viss post i filstrukturen, och kan ge en ytterligare kontext till det digitala materialet.

### dArc
Inom projektet ingick att ta fram ett rudimentärt system för lagring av skivavbildningar samt dess metadata, vilket resulterade i systemet **dArc**. 
#### Funktionalitet
Applikationen har i sin nuvarande **enkla** form följande funktionalitet:
* Möjlighet att skapa en arkivbildare
* Möjlighet att skapa ett arkiv som tillhör en/flera arkivbildare
* Möjlighet att skapa en disk-post
* Möjlighet att införliva skivavbildningar tillsammans med DFXML för en disk-post
* Möjlighet att bläddra i skivavbildningens filstruktur utifrån DFXML
* Möjlighet att söka fram filer och mappar i skivavbildningens filstruktur utifrån DFXML

####Teknisk plattform
Som lagringsplattform valdes fedora-commons (http://www.fedora-commons.org) som är en populär lösning för lagring av fildata.

Till affärslagret av applikationen valdes Ruby on Rails (http://rubyonrails.org), och för presentationen EmberJS (http://www.emberjs.org).
Resultat

####Källkod
Utvecklingen resulterade i tre separerade repositorier som tillsammans skapar en användbar produkt. Observera att systemet är rudimentärt och inte ska ses som en ’out-of-the-box’ produktionsfärdig lösning.
dArc_store ( www.github.com/ub-digit/dArc_store ) - Innehåller en konfigurerad Fedora installation med tillhörande script för datahantering.
dArc ( www.github.com/ub-digit/dArc ) - Innehåller affärslogiken och levererar ett API utåt som pratar med dArc_store som datakälla.
Förvärv av digitala personarkiv och digital forensis 2015-03
16
dArc_ember ( www.github.com/ub-digit/dArc_ember ) - En Frontend-applikation som nyttjar APIer från dArc för att hantera data som lagras i dArc_store.
Samtliga repositorier är helt fria att använda eller vidareutveckla.
Resultat och slutsatser
Mallavtal och checklistor
Liksom vid leveranser av pappersarkiv bör det upprättas en överenskommelse/kontrakt vid digitala arkivleveranser som definierar vilket material som ingår och annan information om förvärvet. Det gäller till exempel vilka rättigheter som följer med förvärvet, behåller donatorn en kopia av hela materialet, hur ska kringinformation