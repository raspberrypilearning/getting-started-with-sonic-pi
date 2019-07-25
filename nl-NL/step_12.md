## Gebruik van rrand

Sonic Pi bevat een aantal functies die meer interessante elementen aan je muziek kunnen toevoegen. Een echt leuke functie is `rrand`, die een waarde tussen twee opgegeven getallen teruggeeft. Voor een cool effect, gebruik `rrand` om de cutoff rond te laten springen.

- Typ in een leeg werkblad:
    
    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: 80
      sleep 0.2
    end
    ```

- In plaats van een getal als `80` aan de cutoff te geven, probeer dan `rrand (40, 120)` zoals hier:
    
    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: rrand(40, 120)
      sleep 0.2
    end
    ```

- Vervolgens kun je gaan experimenteren met `rrand` met andere parameters. Voeg bijvoorbeeld `pan: rrand (-1, 1)` toe aan de regel voor het spelen van akkoorden en druk vervolgens op **Run**.