## Skift lydene

Det er tid til at gøre dine melodier mere interessante! Vi kan gøre dette ved at ændre de brugte synthesizer lyde. Standardsynthen, som Sonic Pi bruger, er kaldt `beep`.

For at bruge en anden synth, bliver du nødt til at tilføje koden `use_synth :navn på synth` over den sekvens af kode, som du vil bruge den i.

I dette eksempel er `fm` navnet af den brugte synth:

```ruby
use_synth :fm
2.times do
  play 60
  sleep 0.5
  play 67
  sleep 0.5
end
```

### Synths, du kan bruge

Der er mange synths, der lyder seje, som er inkluderet med Sonic Pi. For at finde deres navne, klik på **help** ikonet øverst på skærmen for at vise hjælpedokumentationen. Vælg derefter **Synths** fra fanerne til venstre af hjælpevinduet. Klik på en af synth navnene for at få at vide, hvordan man bruger det.

