# Utläsning av data från bärare
Då integriteten hos bärare av digitalt material är osäker i bästa fall, bör dess data lagras på ett säkert sätt i så nära anknytning till att bäraren levereras till arkivet som möjligt. Risken är annars överhängande att viss data helt eller delvis går förlorad. Det finns olika sätt att åstadkomma detta, vilka vardera kommer med sina styrkor och svagheter.

[Läs om att skapa en skivavbildning (digital kopia av den fysiska bäraren)](skivavbildning.md)

[Läs om att kopiera filer från en bärare eller skivavbildning](filkopiering.md)
<hr>
> Data kan läsas direkt från en disk, eller via en skivavbildning. Skivavbildningar är oftast att föredra, men kan ibland vara praktiskt olämpliga på grund av sin storlek.

##Programvara
Det finns en mängd olika programvaror tillgängliga på marknaden, en lista på en del finns tillgänglig i [Projektrapporten](https://github.com/ub-digit/digital-forensis/raw/master/bilagor/projektrapport_forvarv_av_digitala_personarkiv_och_digital_forensis.pdf).

Rekommendationen är dock att börja med att använda [BitCurator](http://wiki.bitcurator.net/index.php?title=Main_Page), som ger tillgång till en mängd programvaror samt rapportverktyg. För att läsa mer om BitCurator projektet, [klicka här](http://www.bitcurator.net/).

BitCurator-sviten kommer att användas som referens i följande guider, men rekommendationerna är inte begränsade till någon specifik programvarusvit.

## Skrivblockerare
För att vara säker på att data inte förvanskas vid kopiering och analys från bäraren används skrivblockerare(eng. Write blocker). Syftet är att säkerställa att ingen data skrivs till bäraren som ska analyseras. 

Skrivningar till bärare kan ske av misstag, men också via den kommunikation som standardmässigt äger rum mellan en dator och dess olika lagringsytor. Det går alltså inte att vara säker på att ingen data skriv till bäraren utan att aktivt använda sig utav en skrivblockerare.

###Mjukvarubaserad skrivblockerare
I många fall kan det räcka med en mjukvarubaserad variant, där en applikation förbjuder operativsystemet att skriva något till bäraren. En sådan variant fungerar bra i dom allra flesta fall, framförallt mot oavsiktlig skrivning. Dock kan en mjukvara aldrig ge en fullständig garanti för att data gålls intakt, då programvaran körs på en högre nivå än ex. operativsystemet eller BIOS, och därmed omöjligen kan ha full kontroll över allt möjligt informationsutbyte.

I BitCurator-sviten ingår en mjukvarubaserad skrivblockerare, som enkelt aktiveras via gränssnittet.

###Hårdvarubaserad skrivblockerare
För att vara helt säker på att ingen data kan skrivas till bäraren, används en hårdvaruvariant av skrivblockerare. Denna består av en dosa som ansluts mellan datorn och bäraren, vilket ger blockeraren möjlighet att se till att ingen information någonsin skickas till bäraren.

<hr>
>Skrivblockerare används för att vara säker på att ingen data skrivs till disken som ska analyseras. Skrivblockerare finns tillgängliga både som programvara och hårdvara.