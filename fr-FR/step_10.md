## Ajouter des effets

Les synthétiseurs modernes ont la possibilité d'ajouter des effets aux sons. Sonic Pi n'est pas différent : tu peux ajouter des effets studio tels que réverbération, écho et distorsion. Bien sûr, tu dois utiliser du code pour ajouter les effets !

- Dans une nouvel espace de travail, trouve un échantillon que tu aimes, par exemple `sample :guit_e_fifths`

- Enveloppe l'échantillon dans un bloc d'effets comme ceci :
    
    ```ruby
    with_fx :reverb do
      sample :guit_e_fifths
    end
    ```

- Tu peux ajouter des effets en plus des effets comme ceci :
    
    ```ruby
    with_fx :reverb do
      with_fx :distortion do
        sample :guit_e_fifths
      end  
    end
    ```

- Joue avec quelques effets et ajoute-les à ta musique. Rappelle-toi qu'une liste complète d'effets peut être trouvée dans la section d'aide de Sonic Pi sous **FX**.