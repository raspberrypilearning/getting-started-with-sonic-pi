## At ændre parametre

Det er muligt, at du nogen gange gerne vil få lyde til at spille i længere tid eller ved en anden hastighed. Dette kan let opnås ved at ændre parametrene af den kode, som du bruger.

Som et eksempel kan vi undersøge `play 60`.

- Klik på **help** for at åbne hjælpedokumentationen. Vælg derefter **lang** på den venstre side, og kør ned til **play**. Du vil blive vist nogle eksempler på, hvordan det bliver brugt. Indtil videre har du brugt `play` uden nogen parametre; lad os bruge nogen nu.
- Skriv i et nyt worksheet:

```ruby
play 60, attack: 1, release: 3
```

- Tryk på **play** knappen for at høre, hvordan den ene node lyder. Attack og release styrer amplituden af en node over tid.

- Prøv nu at ændre værdierne for attack og release for at se, hvordan disse parametre påvirker noden.

Der er mange andre parametre, som også kan ændre, hvordan et sample eller en synth lyder. Prøv at ændre værdierne for `cutoff:`, `pan:`, `rate:`, eller `amp:`.

For at få en fuld liste af parametre, klik på **Help** ikonet, og derefter på **Samples**. Vælg et sample og rul ned for at få en fuld forklaring for hver parameter, der kan bruges med det valgte sample. Det samme gælder også for synths!
