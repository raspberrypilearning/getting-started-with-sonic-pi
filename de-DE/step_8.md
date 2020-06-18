## Zwei Musikstücke gleichzeitig spielen

Musik hat oft ein sich wiederholendes Hintergrundstück mit einer im Vordergrund gespielten, separaten Melodie. In Sonic Pi hast du bisher eine Melodie gespielt. Lasse uns versuchen, zwei Musikstücke gleichzeitig zu spielen!

- Klicke auf eine neue Pufferregisterkarte.

2. Der Code, den wir zur gleichzeitigen Wiedergabe von zwei Musikstücken verwenden, muss zwischen `in_thread do` und `end` stehen.

3. Gebe unter `in_thread do` (auf Deutsch: im Abarbeitungsstrang ausführen) deine Melodie ein. Hier habe ich ein Sample für meinen Hintergrundstück (auch Playback oder backing track genannt) verwendet:
    
    ```ruby
    in_thread do
      loop do
        sample: loop_amen
        sleep 1.753
      end
    end       
    ```
    
    Dieser erste "Thread" (Strang) fungiert als Melodie deiner Musik. Darunter kannst du den Code für dein Hintergrundstück oder Baseline (Tonspur des Basses) eingeben.

4. Tippe:
    
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

5. Drücke jetzt **play** und du solltest beide Stränge gleichzeitig hören.