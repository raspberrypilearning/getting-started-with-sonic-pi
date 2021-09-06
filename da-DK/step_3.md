## Første lyde med Sonic Pi

![](images/GUI.png)

Dette er Sonic Pi interfacet; det har tre hovedvinduer. Det største vindue er til at skrive din kode, og vi vil kalde det Programmeringspanelet. Der er også et output panel, der viser information omkring dit program, mens det kører. Når du klikker på **help** knappen øverst i vinduet, vil det tredje panel dukke op langs bunden og vise hjælpedokumentationen. Dette indeholder information omkring forskelligt kode du kan prøve, så vel som forskellige synth lyde, samples, og meget mere.

- Kør Sonic Pi fra skrivebordet eller applikationsmenuen.

- Vælg **Buffer 1** og skriv:

```ruby
play 60
```

- Klik på **play** ikonet øverst på skærmen. Hvad sker der efterfølgende?

- Hvad sker der, hvis du skriver `pley 60` og trykker på play ikonet?

	Dette er et eksempel på en bug i din kode. I de kommende aktiviteter, hvis error-panelet viser tekst, vil du vide, at du har en bug der skal fikses. Det kunne være, at du har stavet `play` forkert.

- Skriv nu:

```ruby
play 60
play 67
play 69
```

- Klik på play ikonet øverst på skærmen. Hvad sker der nu?

- Computeren afspiller hver node i sekvens (en efter den anden), men det sker så hurtigt, at det for os lyder som om, at de afspilles samtidigt.

	Vi bliver nødt til at fortælle computeren, at den skal holde pause imellem hver node. Vi kan gøre dette ved at skrive følgende kode efter hver `play`:

```ruby
sleep 1
```

Værdien indtastet efter ordet `sleep` forestiller det antal sekunder, computeren skal holde pause. Værdien 1 skal forestille et sekund. Hvad ville du indtaste for halvdelen af et sekund?

- Skriv nu en sekvens af play og sleep for at lave en melody, der lyder sejt!
