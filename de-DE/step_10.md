## Effekte hinzufügen

Moderne Synthesizer können Effekte zu Sounds hinzufügen. Sonic Pi ist nicht anders: Du kannst Studio-Effekte wie Hall (Reverb), Echo und Verzerrung (Distortion) hinzufügen. Natürlich musst du Code verwenden, um die Effekte hinzuzufügen!

- Finde in einem neuen Arbeitsblatt ein Sample, das dir gefällt, zum Beispiel `sample :guit_e_fifths`

- Schließe das Sample in einen Effektblock wie folgt ein:
    
    ```ruby
    with_fx :reverb do
      sample :guit_e_fifths
    end
    ```

- Du kannst Effekte zusätzlich zu diesen Effekten hinzufügen:
    
    ```ruby
    with_fx :reverb do
      with_fx :distortion do
        sample :guit_e_fifths
      end  
    end
    ```

- Spiele mit einigen Effekten herum und füge sie zu deiner Musik hinzu. Beachte, dass du eine vollständige Liste der Effekte in der Hilfe von Sonic Pi unter **FX** findest.