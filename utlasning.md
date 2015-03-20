# Utläsning av data från bärare
Då integriteten hos bärare av digitalt material är osäker i bästa fall, bör dess data lagras på ett säkert sätt i så nära anknytning till att bäraren levereras till arkivet som möjligt. Risken är annars överhängande att viss data helt eller delvis går förlorad. Det finns olika sätt att åstadkomma detta, vilka vardera kommer med sina styrkor och svagheter.

[Läs om att skapa en skivavbildning (digital kopia av den fysiska bäraren)](skivavbildning.md)

[Läs om att kopiera filer från en bärare eller skivavbildning](filkopiering.md)


## Skrivblockerare
För att vara säker på att data inte förvanskas vid kopiering och analys från bäraren används med fördel Skrivblockerare(eng. Write-Blockers). I många fall kan det räcka med en mjukvarubaserad variant, där operativsystemet helt enkelt inte tillåts skriva något till bäraren. För att vara helt säker krävs dock en hårdvaruvariant. Denna kopplas in mellan datorn och bäraren, och ser till att ingen information kan skickas till bäraren.

>Även då du _tror_ att du bara läser data från en disk som är inkopplad till din dator, sker det alltid viss kommunikation tillbaka till disken. För att denna kommunikation påverkar bärarens integritet används Skrivblockerare.