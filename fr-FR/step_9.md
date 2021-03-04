## Coder en direct !

Sonic Pi a été développé pour être une plate-forme pour le codage en direct de la musique, pour que le code puisse être manipulé, modifié et adapté en temps réel ; cela signifie que les codeurs peuvent exécuter leur code plutôt que de jouer des programmes pré-écrits. Pourquoi ne pas essayer ?

- Dans un nouveau onglet tampon :
    
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

- Appuie sur **Run** pour démarrer le programme.

- Pendant que la musique joue, commente les trois dernières lignes en ajoutant un symbole `#` au début de chaque ligne comme ceci :
    
    ```ruby
    # loop do
    #   play_my_synth
    # end
    ```

- Modifie ensuite une partie du code dans la fonction et appuie à nouveau sur **Run**. Maintenant tu es vraiment en train de déchirer !