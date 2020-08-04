## Modifica parámetros

En ocasiones, te gustaría hacer que los sonidos se reproduzcan durante un tiempo más largo o a un ritmo diferente. Esto puede lograrse fácilmente modificando los parámetros del código que estás utilizando.

Toma `play 60`, por ejemplo.

- Haz clic en **help** para abrir los documentos de ayuda, luego selecciona **lang** en el lado izquierdo y baja a **play**. Verás algunos ejemplos de su uso. Hasta ahora has usado `play` sin ningún parámetro; vamos a usar algunos ahora.
- En una nueva hoja de trabajo, escribe:
    
    ```ruby
    play 60, attack: 1, release: 3
    ```

- Presiona el botón **play** para escuchar cómo suena esa nota. Attack y release controlan la amplitud de una nota con el tiempo.

- Ahora cambia los valores para attack y release para ver cómo estos parámetros afectan la nota.

Hay muchos parámetros que también pueden cambiar la forma en que suenan las muestras o los sintetizadores. Intenta cambiar los valores para `cutoff:`, `pan:`, `rate:` o `amp:`.

Para una lista completa de parámetros para cada muestra, haz clic en el ícono **Help**, seguido de **Samples**. Selecciona una muestra y desplázate hacia abajo para ver una explicación completa de cada tipo de parámetro que se puede usar con esa muestra. ¡Lo mismo aplica para los sintetizadores!