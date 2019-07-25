## MIDI notes and music notes

The values that you have been typing after the word `play` represent notes; in fact, they are MIDI note numbers. This means we can translate songs played on a piano into Sonic Pi using a table like so:

`C D E C` or `60 62 64 60` in MIDI notes.

**Music Notes to MIDI Note Values**

| C  | D  | E  | F  | G  | A  | B  |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 60 | 62 | 64 | 65 | 67 | 69 | 71 |

This is quite a long process if you know the notes of the song you are trying to play. With Sonic Pi you are able to use standard sheet music notation too.

- In a new buffer tab type:
    
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

- Press **play** to hear your tune. Does it sound the same as when you used MIDI notes?