## Utiliser rrand

Sonic Pi inclut un certain nombre de fonctions qui peuvent ajouter des éléments plus intéressants à ta musique. Une fonction vraiment amusante est `rrand`, qui retournera une valeur entre deux nombres spécifiés. Pour un effet cool, utilise `rrand` pour faire rebondir la coupure autour de toi.

- Dans un nouvel espace de travail vide :
    
    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: 80
      sleep 0.2
    end
    ```

- Au lieu de passer un nombre comme `80` à la valeur cutoff, essaie `rrand(40, 120)` comme ceci :
    
    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: rrand(40, 120)
      sleep 0.2
    end
    ```

- Ensuite, tu peux commencer à expérimenter en utilisant `rrand` avec d'autres paramètres. Par exemple, ajoute `pan: rrand(-1, 1)` à la ligne play chord, puis appuie sur **Run**.