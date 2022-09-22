## At afspille to melodier på samme tid

Musik har ofte en gentagende baggrundsspor, med en separat melodi der spiller over det. Indtil videre har du spillet én melodi i Sonic Pi. Lad os prøve at afspille to melodier på samme tid!

1. Klik på en ny buffer fane.

2. Den kode, vi bruger til at afspille to melodier samtidigt, er nødt til at være imellem `in_thread do` og `end`.

3. Nedenunder `in_thread do`, indtast din melodi. I dette eksempel har jeg brugt et sample for mit baggrundsspor:

```ruby
in_thread do
  loop do
    sample :loop_amen
    sleep 1.753
  end
end
```

    Denne første 'tråd' vil opføre sig som hovedmelodien af din musik. Under dette kan du skrive koden til dit baggrundsspor eller baseline.

4. Skriv:

```ruby
in_thread do
  16.times do
    play 75
    sleep 1.753
    play 74
    sleep 0.25
  end
end
```

5. Tryk **play** nu, og du burde høre begge tråde blive afspillet samtidigt.
