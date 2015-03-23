# Lagring av data
Digitala filer såsom dokument, skivavbildningar samt dess metadata, som har en anknytning till ett personarkiv eller liknande bör lagras med fullvärdig integritet gällande backuprutiner och dylikt.

## Lagring av skivavbildningar
Då skivavbildningar lagras, är det viktigt att ta hänsyn till den metadata som producerats utifrån skivavbildningen, vanligtvis i form av *DFXML*, som är ett standardformat för att dokumentera skivavbildningar samt dess innehåll.

Då informationen i en skivavbildningfils DFXML innehåller information om filer, filsystem, filstorlek, ändrad-datum, raderade filer et c, är det relevant information att spara på ett säkert vis, oavsett ifall skivavbildningen lagras eller ej.

DFXML ger möjlighet att referera extraherade filer till en viss post i filstrukturen, och kan ge en ytterligare kontext till det digitala materialet.

### dArc
Inom projektet ingick att ta fram ett rudimentärt system för lagring av skivavbildningar samt dess metadata, vilket resulterade i systemet **dArc**