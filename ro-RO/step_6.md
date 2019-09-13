## Modifică sunetele

E timpul să-ți faci melodia mai interesantă! Putem face acest lucru prin schimbarea sintetizatorului pe care îl folosește. Sintetizatorul implicit din Sonic Pi este numit `beep`.

Pentru a folosi un alt sintetizator, trebuie să adaugi codul `use_synth :nume_sintetizator` deasupra secvenței de cod pentru care dorești să îl utilizezi.

În acest exemplu, `fm` este numele sintetizatorului:

```ruby
use_synth :fm
2.times do
  play 60
  sleep 0.5
  play 67
  sleep 0.5
end
```

### Sintetizatoare de încercat

În Sonic Pi sunt incluse o mulțime de sintetizatoare care sună interesant. Pentru a le afla numele, dă click pe pictograma **help** din partea de sus a ecranului, astfel încât să apară fereastra de documentație. Apoi alege **Synths** din filele din partea stângă a ferestrei de ajutor. Dă click pe numele oricăruia dintre sintetizatoare pentru a obține mai multe informații despre cum să îl folosești.