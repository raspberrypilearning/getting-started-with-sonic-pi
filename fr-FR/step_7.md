## Utiliser des échantillons

Non seulement tu pourras créer de la musique dans Sonic Pi en utilisant des notes simples, mais tu peux également créer de la musique avec des échantillons. Les échantillons sont des sons préenregistrés ou des musiques que tu peux apporter dans ta musique. C'est une façon vraiment simple de rendre ta musique incroyable !

Pour utiliser un échantillon, tu dois ajouter le code `sample :name of sample` dans la séquence de ton programme de musique où tu veux qu'il soit joué.

Dans cet exemple, `loop_amen` est le nom de l'échantillon :

```ruby
2.times do
  sample :loop_amen
  sleep 1.753
end
```

### Échantillons à essayer

Il y a beaucoup d'échantillons inclus avec Sonic Pi. Pour trouver leurs noms, clique sur **Help** suivi de **Échantillons** sur le côté gauche de la fenêtre d'aide. Clique sur l'un des noms de l'échantillon pour obtenir plus d'informations sur la façon de l'utiliser.