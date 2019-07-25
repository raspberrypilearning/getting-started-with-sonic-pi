## Effecten toevoegen

Moderne synthesizers hebben de mogelijkheid om effecten toe te voegen aan geluiden. Sonic Pi is niet anders: je kunt studio-effecten toevoegen, zoals galm (reverb), echo en vervorming (distortion). Natuurlijk moet je code gebruiken om de effecten toe te voegen!

- Zoek in een nieuw werkblad een sample die je bevalt, bijvoorbeeld `sample: guit_e_fifths`

- Zet de sample als volgt in een effect blok:
    
    ```ruby
    with_fx :reverb do
      sample :guit_e_fifths
    end
    ```

- Je kunt effecten toevoegen aan effecten zoals hier:
    
    ```ruby
    with_fx :reverb do
      with_fx :distortion do
        sample :guit_e_fifths
      end  
    end
    ```

- Speel wat met enkele effecten en voeg ze toe aan je muziek. Vergeet niet dat een volledige lijst met effecten te vinden is in de help sectie van Sonic Pi onder **Effecten**.