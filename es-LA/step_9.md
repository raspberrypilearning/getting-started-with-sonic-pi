## ¡Código en vivo!

Sonic Pi ha sido desarrollado para ser una plataforma para la codificación en vivo de música, para que el código pueda ser manipulado, modificado y adaptado en tiempo real; esto significa que los codificadores pueden realizar su código en lugar de reproducir programas preescritos. ¿Por qué no intentarlo?

- En una nueva pestaña buffer, escribe:
    
    ```ruby
    define :play_my_synth do
      use_synth :prophet
      play 50, attack: 0.2, release: 1.3
      sleep 0.5
    end
    
    loop do
      play_my_synth
    end
    ```

- Presiona **play** para empezar el programa.

- Mientras la melodía está sonando, comenta las tres últimas líneas añadiendo un símbolo `#` al inicio de cada línea, de esta manera:
    
    ```ruby
    # loop do
    #   play_my_synth
    # end
    ```

- Luego cambia algo de código en la función y presiona **play** de nuevo. ¡Ahora estás realmente rockeando!