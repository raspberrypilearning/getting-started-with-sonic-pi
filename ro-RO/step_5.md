## Note MIDI și note muzicale

Valorile pe care le-ai introdus după cuvântul `play` reprezintă note; de fapt, sunt numere asociate notelor MIDI. Acest lucru înseamnă că putem traduce melodii cântate la pian în Sonic Pi folosind un tabel ca acesta:

`C D E C` sau `60 62 64 60` folosind notele MIDI.

**De la note muzicale la note MIDI**

| C (Do) | D (Re) | E (Mi) | F (Fa) | G (Sol) | A (La) | B (Si) |
|:------:|:------:|:------:|:------:|:-------:|:------:|:------:|
|   60   |   62   |   64   |   65   |   67    |   69   |   71   |

Acesta este un proces destul de lung dacă știi notele piesei pe care încerci să o redai. Dar cu Sonic Pi poți folosi și notația muzicală standard.

- Într-o filă buffer nouă scrie:
    
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

- Apasă **play** pentru a asculta melodia. Sună la fel ca atunci când ai folosit note MIDI?