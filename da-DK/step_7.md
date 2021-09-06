## Brug samples

Ikke nok med at du kan lave musik i Sonic Pi ved at bruge enkelte noder, men du kan også lave musik med samples. Samples er forudindspillede lyde eller melodier, som du kan indsætte i din musik. Dette er en meget simpel måde at få din musik til at lyde utroligt godt!

For at bruge en sample, skal du tilføje koden `sample :navn af sample` i den sekvens af dit musikprogram, hvor du vil have det til at blive afspillet.

I dette eksempel er `loop_amen` navnet på det brugte sample:

```ruby
2.times do
  sample :loop_amen
  sleep 1.753
end
```

### Samples, du kan bruge

Der er mange samples inkluderet med Sonic Pi. For at finde deres navne, klik på **help** og derefter **samples** til venstre af hjælpevinduet. Klik på en af sample navnene for at få at vide, hvordan man bruger det.

