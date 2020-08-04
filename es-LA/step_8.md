## Reproduce dos canciones al mismo tiempo

La música a menudo tiene una pista de apoyo repetida, con una melodía separada que se toca sobre la parte superior. Hasta ahora en Sonic Pi has tocado una canción. Hay que intentar reproducir dos canciones al mismo tiempo!

- Haz clic en una nueva pestaña buffer.

2. El código que usamos para reproducir dos canciones al mismo tiempo debe estar entre `in_thread do` y `end`.

3. Debajo de `in_thread do`, escribe tu canción. Aquí he usado una muestra para mi pista de respaldo:
    
    ```ruby
    in_thread do
      loop do
        sample :loop_amen
        sleep 1.753
      end
    end       
    ```
    
    Este primer "hilo" actuará como la melodía de tu música. Debajo, puedes escribir el código para tu pista de respaldo o línea de base.

4. Escribe:
    
    ```ruby
    in_thread do
      16.times do
        play 75
        sleep 1.753
        play 74
        sleep 0.25
      end
    end 
    ```

5. Ahora presiona ** reproducir ** y deberías escuchar los dos hilos reproduciéndose al mismo tiempo.