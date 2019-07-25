## Verander de geluiden

Het is tijd om je deuntje interessanter te laten klinken! We kunnen dit doen door de synthesizergeluiden die het gebruikt te veranderen. De standaard Sonic Pi-synthesizer wordt `beep` genoemd.

Om een ​​andere synth te gebruiken, moet je de code `use_synth: naam van de synth` toevoegen boven de regels code waarin je hem wilt gebruiken.

In dit voorbeeld is `fm` de naam van de synthesizer:

```ruby
use_synth :fm
2.times do
  play 60
  sleep 0.5
  play 67
  sleep 0.5
end
```

### Synths om te proberen

Er zijn veel cool klinkende synths meegeleverd met Sonic Pi. Om de namen ervan te vinden, klik je op het **Help** pictogram aan de bovenkant van het scherm, zodat het venster Help-documenten verschijnt. Selecteer vervolgens **Synthesizers** via de tabbladen onder het Help-venster. Klik op een van de synth-namen voor meer informatie over het gebruik ervan.