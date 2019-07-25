## MIDI-noten en muzieknoten

De waarden die je na het woord `play` hebt getypt vertegenwoordigen noten; in feite zijn het MIDI-nootnummers. Dit betekent dat we liedjes die op een piano worden gespeeld kunnen vertalen naar Sonic Pi met behulp van een tabel zoals:

`C D E C` of `60 62 64 60` in MIDI-noten.

**Muzieknoten omzetten naar MIDI-nootwaarden**

| C  | D  | E  | F  | G  | A  | B  |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 60 | 62 | 64 | 65 | 67 | 69 | 71 |

Dit is best een flink karwei als je de noten van het liedje dat je probeert te spelen kent. Met Sonic Pi kun je ook de standaard bladmuzieknotatie gebruiken.

- In een nieuw buffer tab typ:
    
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

- Druk op **Run** om je deuntje te horen. Klinkt het hetzelfde als toen je MIDI-noten gebruikte?