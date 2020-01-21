## Twee liedjes tegelijkertijd spelen

Muziek heeft vaak een herhalende achtergrondtrack, met een afzonderlijke melodie die er overheen wordt gespeeld. Tot nu toe heb je in Sonic Pi één deuntje gespeeld. Laten we proberen tegelijkertijd twee deuntjes te spelen!

- Klik op een nieuw buffer tabblad.

2. De code die we gebruiken om tegelijkertijd twee deuntjes te spelen, moet tussen `in_thread do` en `end` geplaatst worden.

3. Onder `in_thread do`, typ je jouw melodie. Hier heb ik een sample gebruikt voor mijn achtergrondtrack:
    
    ```ruby
    in_thread do
      loop do
        sample :loop_amen
        sleep 1.753
      end
    end       
    ```
    
    Deze eerste 'thread' zal fungeren als de melodie van je muziek. Hieronder kun je de code voor je achtergrondtrack of basislijn typen.

4. Typ:
    
    ```ruby
    in_thread do
      16.times do
        play 75
        sleep 1.753
        play 74
        sleep 0.25
      end
    end 
    ```

5. Druk nu op **play** en je zou beide threads op hetzelfde moment moeten horen.