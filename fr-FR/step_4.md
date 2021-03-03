## Boucler une musique

Maintenant que tu as maîtrisé les bases de Sonic Pi, allons coder une musique !

- Sélectionne **Tampon 2**.

2. Tape le code suivant :
    
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

3. Maintenant, clique sur l'icône Run en haut de l'écran et il jouera la première partie de la musique. Peux-tu dire ce que c'est ?
    
    *Réponse : Frère Jacques !*
    
    Cette première section joue deux fois. Comment pourrais-tu la répéter ? Tu peux taper à nouveau la même section, ou nous pourrions commencer à introduire des boucles dans ton code.

4. En haut de ton code, au-dessus du premier `play 60`, tape :
    
    ```ruby
    2.times do
    ```

5. Et en bas de ton code, ci-dessous `sleep 0.5`, tape :
    
    ```ruby
    end
    ```

6. Clique sur l'icône Run en haut de l'écran. Que se passe-t-il ?
    
    Jouons cette partie dans Sonic Pi.
    
    Dans l'exemple ci-dessous, tu peux voir que certaines lignes de code sont indentées. Il est ainsi plus facile de lire ton code et de vérifier s'il ne fonctionne pas lorsque tu appuies sur le bouton Run. Tu peux appuyer deux fois sur la barre d'espace pour indenter une ligne de code.
    
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

### Boucler indéfiniment ?

Boucler des notes pour un certain nombre de fois est certainement utile, mais que faire si tu veux boucler ta musique indéfiniment ?

Au lieu d'utiliser `2.times do` et `end` tu peux utiliser `loop do` et `end`, comme ceci :

```ruby
loop do
  play 60
  sleep 0.5
end
```