## Herhaal een deuntje

Nu heb je de basis van Sonic Pi onder de knie, laten we een deuntje coderen!

- Selecteer **Buffer 2**.

2. Typ de volgende code:
    
    ```ruby
    play 60
    sleep 0.5
    play 62
    sleep 0.5
    play 64
    sleep 0.5
    play 60
    sleep 0.5
    ```

3. Klik nu op het afspeelpictogram bovenaan het scherm en het speelt het eerste deel van een deuntje. Kun je vertellen wat het is?
    
    *Antwoord: Vader Jacob!*
    
    Dit eerste gedeelte wordt twee keer gespeeld. Hoe kun je het herhalen? Je zou hetzelfde gedeelte opnieuw kunnen typen, of we zouden loops (lussen) in je code kunnen introduceren.

4. Typ bovenaan je code, boven de eerste `play 60`:
    
    ```ruby
    2.times do
    ```

5. En onderaan je code, onder de `sleep 0,5`, type je:
    
    ```ruby
    end
    ```

6. Klik op het Run pictogram bovenaan het scherm. Wat gebeurt er?
    
    Laten we dit deel in Sonic Pi spelen.
    
    In het onderstaande voorbeeld kun je zien dat sommige regels code zijn ingesprongen. Dit maakt het makkelijker om je code te lezen, en eventuele fouten op te lossen, als deze niet werkt wanneer je op de afspeelknop drukt. Je kunt twee keer op de spatiebalk drukken om een ​​coderegel in te springen.
    
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

### Voor altijd herhalen?

Noten gedurende een bepaald aantal keren herhalen is zeker handig, maar wat als je je deuntje voor altijd wilt herhalen?

In plaats van `2.times do` en `end` kun je `loop do` en `end` gebruiken, zoals hier:

```ruby
loop do
  play 60
  sleep 0.5
end
```