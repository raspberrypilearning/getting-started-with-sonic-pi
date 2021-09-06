## Live kode!

Sonic Pi er blevet udviklet til at være en platform for live kodning af music, så koden kan blive manipuleret, ændret, og tilpasset i realtid; dette betyder, at programmører kan udføre deres kode i stedet for at afspille forudskrevet programmer. Lad os prøve det!

- I en ny buffer fane, skriv:

```ruby
define :play_my_synth do
	use_synth :prophet
	play 50, attack: 0.2, release: 1.3
	sleep 0.5
end

loop do
	play_my_synth
end
```

- Tryk **play** for at starte programmet.
- Mens melodien spiller, kommenter de tre sidste linjer ud ved at tilføje et `#` symbol i starten af hver linje som vist her:

```ruby
# loop do
#   play_my_synth
# end
```

- Lav derefter nogle ændringer til noget af koden i funktionen og tryk **play** igen. Nu rocker du for vildt!
