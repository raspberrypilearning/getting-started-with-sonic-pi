## Changer les sons

Il est temps de rendre ta musique plus intéressante ! Nous pouvons le faire en modifiant les sons du synthétiseur qu'il utilise. Le synthé Sonic Pi par défaut est appelé `beep`.

Pour utiliser un synthé différent, tu dois ajouter le code `use_synth :name of synth` au-dessus de la séquence de code dans laquelle tu veux l'utiliser.

Dans cet exemple, `fm` est le nom du synthé :

```ruby
use_synth :fm
2.times do
  play 60
  sleep 0.5
  play 67
  sleep 0.5
end
```

### Synthés à essayer

Il y a beaucoup de synthés cool inclus avec Sonic Pi. Pour trouver leurs noms, clique sur l'icône **Help** en haut de l'écran pour que la fenêtre de documents d'aide apparaisse. Puis sélectionne **synthétiseur** dans les onglets le long du côté gauche de la fenêtre d'aide. Clique sur l'un des noms de synthé pour obtenir plus d'informations sur la façon de l'utiliser.