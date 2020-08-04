## Utiliza rrand

Sonic Pi incluye una serie de funciones que pueden añadir elementos más interesantes a tu música. Una función realmente divertida es `rrand`, que devolverá un valor entre dos números especificados. Para un efecto genial, usa `rrand` para hacer el rebote de corte.

- En una nueva hoja de trabajo, escribe:
    
    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: 80
      sleep 0.2
    end
    ```

- En lugar de pasar un número como `80` al valor de corte, prueba `rrand(40, 120)` así:
    
    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: rrand(40, 120)
      sleep 0.2
    end
    ```

- Entonces puedes empezar a experimentar usando `rrand` con otros parámetros. Por ejemplo, añade `pan: rrand(-1, 1)` a la línea de código play chord y luego presiona **play**.