## Modifier les paramètres

Parfois, tu aimerais faire jouer des sons plus longtemps ou à un rythme différent. Cela peut être réalisé facilement en modifiant les paramètres du code que tu utilises.

`play 60`, par exemple.

- Clique sur **Help** pour ouvrir les documents d'aide. puis sélectionne **lang** sur le côté gauche et descends jusqu'à **play**. Tu verras quelques exemples de son utilisation. Jusqu'à présent, tu as utilisé `play` sans aucun paramètre ; nous allons en utiliser un.
- Dans un nouvel espace de travail :
    
    ```ruby
    play 60, attack: 1, release: 3
    ```

- Appuie sur le bouton **Run** pour entendre comment cette note sonne. Attack et release contrôlent l'amplitude d'une note au fil du temps.

- Change maintenant les valeurs attack et release pour voir comment ces paramètres affectent la note.

Il existe de nombreux paramètres qui peuvent également modifier le son des échantillons ou des synthés. Essaie de changer les valeurs pour `cutoff:`, `pan:`, `rate:` ou `amp:`.

Pour une liste complète des paramètres pour chaque échantillon, clique sur l'icône **Help** suivie de **Échantillons**. Sélectionne un échantillon et fais défiler vers le bas pour voir une explication complète pour chaque type de paramètre qui peut être utilisé avec cet échantillon. Il en va de même pour les synthés !