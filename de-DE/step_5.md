## MIDI-Noten und Musiknoten

Die Werte, die du nach dem Wort `play` eingegeben hast, stehen für Noten. Tatsächlich handelt es sich um MIDI-Notennummern. Dies bedeutet, dass wir auf einem Piano gespielte Songs in Sonic Pi mit einer Tabelle wie folgt übersetzen können:

`C D E C` oder `60 62 64 60` in MIDI-Noten.

**Musiknoten zu MIDI-Notenwerten**

| C  | D  | E  | F  | G  | A  | B  |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 60 | 62 | 64 | 65 | 67 | 69 | 71 |

Dies ist ein ziemlich langer Prozess, wenn du die Noten des Songs kennst, den du zu spielen versuchst. Mit Sonic Pi kannst du auch die Standardnotenschrift verwenden.

- In einer neuen Puffer-Registerkarte (Englisch: Buffer):
    
    ```ruby
    play :c4
    sleep 0.5
    play :d4
    sleep 0.5
    play :e4
    sleep 0.5
    play :c4
    sleep 0.5
    ```

- Drücke **play** um deine Melodie zu hören. Klingt es genauso wie bei der Verwendung von MIDI-Noten?