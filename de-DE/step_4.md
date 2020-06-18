## Wiederhole eine Melodie

Jetzt beherrscht du die Grundlagen von Sonic Pi. Lass uns eine Melodie programmieren!

- Wähle **Buffer 2**.

2. Geben den folgenden Code ein:
    
    ```ruby
    play 60
    sleep 0,5
    play 62
    sleep 0,5
    play 64
    sleep 0,5
    play 60
    sleep 0,5
    ```

3. Klicke nun auf das Wiedergabesymbol oben auf dem Bildschirm, um den ersten Teil einer Melodie abzuspielen. Kannst du sagen, was es ist?
    
    *Antwort: Bruder Jakob!*
    
    Dieser erste Abschnitt wird zweimal gespielt. Wie kannst du es wiederholen? Du könntest den gleichen Abschnitt erneut eingeben, oder wir könnten damit beginnen, Schleifen (Loops) in deinen Code einzuführen.

4. Gebe oben in deinen Code über den ersten `play 60` folgendes ein:
    
    ```ruby
    2.times do 
    (auf Deutsch: zwei Mal tun)
    ```

5. Und gebe unten in deinem Code unter `sleep 0.5` folgendes ein:
    
    ```ruby
    end 
    (auf Deutsch: Ende)
    ```

6. Klicke auf das Wiedergabesymbol oben auf dem Bildschirm. Was geschieht?
    
    Lass uns diesen Teil in Sonic Pi spielen.
    
    Im folgenden Beispiel siehst du, dass einige Codezeilen eingerückt sind. Dies macht es einfacher, deinen Code zu lesen und nach Fehlern zu suchen, wenn er beim Drücken der Wiedergabetaste nicht funktioniert. Du kannst die Leertaste zweimal drücken, um eine Codezeile einzurücken.
    
    ```ruby
    2.times do
      play 60
      sleep 0.5
      play 62
      sleep 0.5
      play 64
      sleep 0.5
      play 60
      sleep 0.5
    end
    ```

### Ewige Schleife?

Das Durchlaufen von Noten für eine festgelegte Anzahl von Malen ist sicherlich nützlich, aber was ist, wenn du deine Melodie für immer durchspielen möchtest?

Anstelle von `2.times do` und `end` kannst du `loop do` und `end`, wie folgt benutzen:

```ruby
loop do
  play 60
  sleep 0.5
end
```