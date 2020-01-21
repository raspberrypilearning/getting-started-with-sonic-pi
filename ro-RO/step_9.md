## Programare live!

Sonic Pi a fost dezvoltat pentru a fi o platformă pentru redarea live a muzicii prin cod, astfel încât acesta să poată fi manipulat, schimbat și adaptat în timp real; acest lucru înseamnă că un programator/artist pot interpreta live folosind codul în loc să redea programe scrise anterior. De ce să nu incerci?

- Într-un tab de tip new buffer:
    
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

- Apasă **play** pentru a porni programul.

- În timp ce melodia este redată, comentează ultimele trei linii prin adăugarea unui simbol `#` la începutul lor astfel:
    
    ```ruby
    # loop do
    #   play_my_synth
    # end
    ```

- Next change some of code in the function, and press **play** again. Now you are really rocking!