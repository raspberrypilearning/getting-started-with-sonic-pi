## Parameters wijzigen

Soms wil je geluiden misschien langer of met een ander tempo laten spelen. Dit kan eenvoudig worden bereikt door de parameters van de code die je gebruikt te wijzigen.

Neem bijvoorbeeld `play 60`.

- Klik op **Help** om de Help-documenten te openen, selecteer vervolgens **Taal** aan de linkerkant en scrol omlaag naar **play**. Je zult enkele voorbeelden van het gebruik ervan zien. Tot nu toe heb je `play` zonder parameters gebruikt; laten we er nu een paar gebruiken.
- Typ in een nieuw werkblad:
    
    ```ruby
    play 60, attack: 1, release: 3
    ```

- Druk op de **Run** knop om te horen hoe die ene noot klinkt. Attack (aanval) en release (loslaten) bepalen de amplitude van een noot in de loop van de tijd.

- Wijzig nu de waarden voor attack en release om te zien hoe deze parameters van invloed zijn op de noot.

Er zijn veel parameters die ook de manier waarop samples of synths klinken kunnen veranderen. Probeer de waarden voor `cutoff:`, `pan:`, `rate:` of `amp:` te veranderen.

Klik voor een volledige lijst met parameters voor elk sample op het pictogram **Help**, gevolgd door **Samples**. Selecteer een sample en scrol naar beneden voor een volledige uitleg voor elk type parameter dat met die sample kan worden gebruikt. Hetzelfde geldt voor synths!