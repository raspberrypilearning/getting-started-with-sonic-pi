## Notas MIDI y notas musicales

Los valores que has estado escribiendo después de la palabra `play` representan notas; de hecho, son números de nota MIDI. Esto significa que podemos convertir las canciones reproducidas en un piano a Sonic Pi usando una tabla como esta:

`C D E C` o `60 62 64 60` en notas MIDI.

**Notas musicales a Valores de nota MIDI**

| C  | D  | E  | F  | G  | A  | B  |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 60 | 62 | 64 | 65 | 67 | 69 | 71 |

Este es un proceso bastante largo si conoces las notas de la canción que estás intentando reproducir. Con Sonic Pi también puedes utilizar la notación de partituras estándar.

- En una nueva pestaña buffer escribe:
    
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

- Presiona **play** para escuchar tu melodía. ¿Suena lo mismo que cuando usas notas MIDI?