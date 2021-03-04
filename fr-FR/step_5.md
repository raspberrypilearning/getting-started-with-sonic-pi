## Notes MIDI et notes musicales

Les valeurs que tu as tapé après le mot `play` représentent des notes ; en fait, ce sont des numéros de note MIDI. Cela signifie que nous pouvons traduire les chansons jouées sur un piano en Sonic Pi en utilisant une table comme celle-ci :

`C D E C` or `60 62 64 60` en notes MIDI.

**Notes musicales vers les valeurs des notes MIDI**

| C  | D  | E  | F  | G  | A  | B  |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 60 | 62 | 64 | 65 | 67 | 69 | 71 |

C'est un processus assez long si tu connais les notes de la chanson que tu essaies de jouer. Avec Sonic Pi, tu peux également utiliser la notation de partitions standard.

- Dans un nouveau type d'onglet de tampon :
    
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

- Appuie sur **play** pour écouter ta musique. Le son est-il le même que lorsque tu utilisais des notes MIDI ?