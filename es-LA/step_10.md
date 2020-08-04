## Añade efectos

Los sintetizadores modernos tienen la capacidad de agregar efectos a los sonidos. Sonic Pi no es diferente: puedes añadir efectos de estudio como reverberación, eco y distorsión. ¡Por supuesto que tienes que usar código para añadir los efectos!

- En una nueva hoja de trabajo, encuentra una muestra que te guste, por ejemplo `sample :guit_e_fifths`

- Envuelve la muestra en un bloque de efectos como este:
    
    ```ruby
    with_fx :reverb do
      sample :guit_e_fifths
    end
    ```

- Puedes añadir efectos sobre efectos como este:
    
    ```ruby
    with_fx :reverb do
      with_fx :distortion do
        sample :guit_e_fifths
      end  
    end
    ```

- Prueba con algunos efectos y añádelos a tu música. Recuerda que puedes encontrar una lista completa de efectos en la sección de ayuda de Sonic Pi en **FX**.