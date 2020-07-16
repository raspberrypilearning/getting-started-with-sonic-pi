## Live-Code!

Sonic Pi wurde als Plattform für die Live-Codierung von Musik entwickelt, sodass der Code in Echtzeit manipuliert, geändert und angepasst werden kann. Dies bedeutet, dass Codierer ihren Code ausführen können, anstatt zuvor geschriebene Programme abzuspielen. Warum nicht mal ausprobieren?

- In einer neuen Puffer-Registerkarte:
    
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

- Drücke **play** um das Programm zu starten.

- Während die Melodie abgespielt wird, kommentierst du die letzten drei Zeilen aus, indem du am Anfang jeder Zeile ein `#` Symbol hinzufügst:
    
    ```ruby
    # loop do
    #    play_my_synth
    # end
    ```

- Als nächstes ändere den Code in der Funktion und drücke **play** erneut. Jetzt rockst du wirklich!