## Rrand verwenden

Sonic Pi enthält eine Reihe von Funktionen, mit denen Du deiner Musik weitere interessante Elemente hinzufügen kannst. Eine wirklich lustige Funktion ist `rrand`, die einen Wert zwischen zwei angegebenen Zahlen zurückgibt. Um einen coolen Effekt zu erzielen, verwenden Sie `rrand`, um die Cutoff-Frequenz zu variieren.

- Gib in ein leeres Arbeitsblatt ein:
    
    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: 80
      sleep 0.2
    end
    ```

- Anstatt eine Zahl wie `80` für den Cutoff-Wert (Grenzfrequenz) zu übergeben, versuche `rrand (40, 120)` wie folgt:
    
    ```ruby
    loop do
      play chord (: a3, :minor).choose, attack: 0, release: 0.3, cutoff: rand (40, 120)
      sleep 0.2
    end
    ```

- Dann kannst du mit anderen Parametern für `rrand` experimentieren. Füge beispielsweise `pan: rrand (-1, 1)` zur Play-Akkordlinie hinzu und drücke **play**.