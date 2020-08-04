## Buclear una melodía

Ahora que haz dominado los conceptos básicos de Sonic Pi, ¡codifiquemos una melodía!

- Selecciona **Buffer 2**.

2. Escribe el siguiente código:
    
    ```ruby
    play 60
    sleep 0.5
    play 62
    sleep 0.5
    play 64
    sleep 0.5
    play 60
    sleep 0.5
    ```

3. Ahora haz clic en el ícono de reproducción en la parte superior de la pantalla y reproducirá la primera parte de una melodía. ¿Puedes decirnos lo que es?
    
    *Respuesta: Frère Jacques!*
    
    Esta primera sección se reproduce dos veces. ¿Cómo podría repetirlo? Puedes volver a escribir la misma sección, o podríamos empezar a introducir bucles en tu código.

4. En la parte superior de tu código, arriba del primer `play 60`, escribe:
    
    ```ruby
    2.times do
    ```

5. Y en la parte inferior de tu código, debajo de `sleep 0.5`, escribe:
    
    ```ruby
    end
    ```

6. Haz clic en el ícono de reproducción en la parte superior de la pantalla. ¿Qué ocurre?
    
    Vamos a reproducir esta parte en Sonic Pi.
    
    En el ejemplo siguiente, puedes ver que algunas líneas de código están indentadas. Lo que hace más fácil leer tu código, y verificar si hay errores y si no funciona cuando presionas el botón de reproducción. Puedes presionar la barra espaciadora dos veces para indentar una línea de código.
    
    ```ruby
    2.times do
      play 60
      sleep 0.5
      play 62
      sleep 0.5
      play 64
      sleep 0.5
      play 60
      sleep 0.5
    end
    ```

### Repetir indefinidamente?

Repetir notas por un número determinado de veces es ciertamente útil, pero ¿Qué pasa si quieres repetir tu canción indefinidamente?

En lugar de usar `2.times do` y `end` puedes usar `loop do` y `end`, así:

```ruby
loop do
  play 60
  sleep 0.5
end
```