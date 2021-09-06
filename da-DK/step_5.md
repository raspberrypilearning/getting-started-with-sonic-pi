## MIDI noder og musiknoder

Værdierne du har indtastet efter ordet `play` skal forestille noder; de er faktisk MIDI nodetal. Dette betyder, at vi kan oversætte sange, der er spillet på et klaver, til Sonic Pi MIDI noder ved at bruge en tabel som denne:

`C D E C` eller `60 62 64 60` i MIDI noder.

**Musiknoder til MIDI noder Værdier**

| C       | D      | E     | F     | G     | A     | B     |
| :-----: |:------:|:-----:|:-----:|:-----:|:-----:|:-----:|
| 60      | 62     | 64    | 65    | 67    | 69    | 71    |

Dette er en ret lang proces, hvis du kender noderne til den sang, du prøver at spille. Med Sonic Pi kan du også bruge normal nodenotation.

- I en ny buffer fane, skriv:

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

- Tryk **play** for at høre din melodi. Er melodien den samme som den, du fik ved at bruge MIDI noder?
