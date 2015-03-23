# Skivavbildning
Inom Digital Forensis är det standard att skapa en skivavbildning på materialet så fort som möjligt. Detta innebär i praktiken att en exakt kopia skapas som en enskild fil, vilken sedan kan lagras på ett säkert sätt och analyseras vid ett senare tillfälle. Samtidigt så kan skapandet av en skivavbildning vara väldigt resurskrävande både vad gäller processorkraft, lagringskapacitet och tid.

## Att skapa en skivavbildning
Det finns ett antal programvaror för att skapa en skivavbildning utifrån en bärare, varav Guymager som ingår i BitCurator-sviten är ett exempel. [Klicka här för att komma till BitCurators wiki-sida om Guymager.](http://wiki.bitcurator.net/index.php?title=Creating_a_Disk_Image_Using_Guymager)

>Guymager som ingår i BitCurator sviten ger användaren möjlighet att skapa en Skivavbildning både som RAW-fil eller inkapslad via Expert Witness standarden. 

## Filformat
Det finns ett antal olika format för skapande av skivavbildningar, framförallt då större programvarusviter används. Vinsten med dessa format kan återfinnas i dess kompressionsmöjligheter samt metadata-fält. Dock rekommenderas _RAW-formatet_ som arkiveringsformat, ifall det inte finns en uttryckt tanke med att använda något annat format.

En anledning till detta är att de övriga formaten tagits fram utifrån ett kriminaltekniskt perspektiv, vilket innebär att den metadata som kapsas in tillsammans med skivavbildningen inte nödvändigtvis tillgodoser behoven som finns för en arkivinstitution.

En ytterligare anledning till att rekommendationen faller på RAW-formatet är att de övriga formaten ofta är knutna till företag eller organisationer, där det inte finns någon garanti för att formatet kommer att fortleva under någon längre tidsperiod. Risken finns därmed att arkivet över tid tvingas byta format, och därmed migrera existerande skivavbildningar, eller hantera olika typer av format.

> RAW-formatet är en bit-för-bit kopia av disken, men helt utan tillhörande metadata. Detta lagras istället med tillhörande filer, vanligtvis som XML.

## Metadata
Metadata om en skivavbildning kan bäddas in i den resulterade filen när det gäller vissa filformat. Detta gäller dock inte RAW-formatet, därav är rekommendationen att metadata sparas strukturerat(ex. XML) tillsammans med skivavbildningen.

##Fördelar
* Ger en exakt kopia på ursprungsmaterialet, vilket möjliggör att:
 * Analys kan ske vid ett senare tillfälle utan att man riskerar att ha missat att spara relevant information.
 * Den ursprungliga arbetsmiljön kan virtuellt simuleras i efterhand.
* Skivavbildningen kan agera _auktoritet_ då digitala filer som plockats från bäraren ska referera till en ursprungskälla.

##Nackdelar
* Tar lång tid att skapa för stora diskar.
* Tar upp stor lagringsyta, då skivavbildningen blir lika stor som ursprungsdisken i ett okomprimerat läge.
* Kan ge upphov till rättighetsbekymmer, då många hårddiskar från persondatorer innehåller proprietär data såsom programvaror, spel, e-post et c.