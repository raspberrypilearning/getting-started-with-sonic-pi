## Cambia los sonidos

¡Es hora de hacer que tu melodía suene más interesante! Podemos hacer esto al cambiar los sonidos del sintetizador que estas usando. El sintetizador Sonic Pi predeterminado se llama `beep`.

Para usar un sintetizador diferente, debes agregar el código `use_synth :name of synth` encima de la secuencia del código en la que deseas usarlo.

En este ejemplo, `fm` es el nombre del sintetizador:

```ruby
use_synth :fm
2.times do
  play 60
  sleep 0.5
  play 67
  sleep 0.5
end
```

### Sintetizadores para probar

Sonic Pi contiene muchos sintetizadores geniales. Para encontrar los nombres de ellos, haz clic en el icono **ayuda** en la parte superior de la pantalla para que aparezca la ventana de documentos de ayuda. Luego selecciona **Sintetiza** en las pestañas a lo largo del lado izquierdo de la ventana de ayuda. Haga clic en cualquiera de los nombres de sintetizador para obtener más información sobre cómo usarlo.