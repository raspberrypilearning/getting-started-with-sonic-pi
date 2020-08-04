## Usa muestras

No solo puedes crear música en Sonic Pi usando notas simples, también puedes crear música con muestras. Las muestras son sonidos o melodías pregrabados que puedes incluir en tu música. ¡Esta es una forma muy simple de hacer que tu música suene increíble!

Para usar una muestra, necesitas añadir el código `muestra :name de la muestra` en la secuencia de tu programa de música donde quieras que suene.

En este ejemplo, `loop_amen` es el nombre del sintetizador:

```ruby
2.times do
  sample :loop_amen
  sleep 1.753
end
```

### Muestras para probar

Sonic Pi contiene muchos sintetizadores geniales. Para encontrar los nombres de ellos, haz clic en **ayuda** seguido de **muestras** en el lado izquierdo de la ventana de ayuda. Haga clic en cualquiera de los nombres de muestra para obtener más información sobre cómo usarlo.