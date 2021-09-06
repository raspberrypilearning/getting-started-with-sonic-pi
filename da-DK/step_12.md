## At bruge rrand

Sonic Pi inkluderer et antal funktioner, der kan tilføje mere interessante elementer til din musik. En virkelig sjov funktion er `rrand`, som vil sende en tilfældig værdi mellem to bestemte tal tilbage. Hvis du vil have en sej effekt, kan du bruge `rrand` til at få cutoff til at hoppe rundt.

- Skriv i et tomt worksheet:

    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: 80
      sleep 0.2
    end
    ```
    
- I stedet for at bruge et tal som `80` til at bestemme cutoff værdien, prøv at bruge `rrand(40, 120)` som set her:

    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: rrand(40, 120)
      sleep 0.2
    end
    ```
    
- Du kan derefter eksperimentere med at bruge `rrand` med andre parametre. For eksempel, tilføj `pan: rrand(-1, 1)` til play chord linjen og derefter tryk **play**.    

