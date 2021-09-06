## Gentag en melodi

Nu hvor du har mestret det grundlæggende ved Sonic Pi, lad os kode en melodi!

1. Vælg **Buffer 2**.

2. Indtast følgende kode:

```ruby
play 60
sleep 0.5
play 62
sleep 0.5
play 64
sleep 0.5
play 60
sleep 0.5
```

3. Klik nu på play ikonet øverst på skærmen, og det vil spille den første del af en melodi. Kan du gætte, hvad det er?

	*Svar: Frère Jacques! (Mester Jakob på dansk)*

    Denne første del spilles to gange. Hvordan kan du få det til at gentage sig? Du kunne skrive den samme del igen, men i stedet vil vi starte med at introducere loops til din kode.

4. Øverst i din kode, over den første `play 60`, skriv:

```ruby
2.times do
```

5. Og nederst i din kode, under den sidste `sleep 0.5`, skriv:

```ruby
end
```

6. Klik på play ikonet øverst på skærmen. Hvad sker der?

    Lad os afspille denne del i Sonic Pi.

    I nedenstående eksempel, kan du se at nogle af linjerne er indrykket. Dette gør det lettere at læse din kode, og at finde bugs, hvis det ikke virker når du klikker på play knappen. For at lave indrykning, kan du taste mellemrum to gange.

```ruby
2.times do
    play 60
    sleep 0.5
    play 62
    sleep 0.5
    play 64
    sleep 0.5
    play 60
    sleep 0.5
end
```

### Gentag for evigt?

Det er helt klart nyttigt at gentage melodier et bestemt antal gange, men hvad nu hvis du vil have din melodi til at blive gentaget for evigt?
I stedet for at bruge `2.times do` og `end` kan du bruge `loop do` og `end`, som vist her:

```ruby
loop do
  play 60
  sleep 0.5
end
```
