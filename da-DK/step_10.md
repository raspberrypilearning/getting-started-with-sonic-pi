## At tilføje effekter

Moderne synthesizere kan tilføje effekter til lyde. Sonic Pi er ikke anderledes på det punkt: du kan tilføje studioeffekter som rumklang, ekko, og forvrængning. For at tilføje effekterne bliver du selvfølgelig nødt til at bruge kode!

- Åben et nyt worksheet og find et sample som du synes godt om, for eksempel `sample :guit_e_fifths`

- Indsæt dit sample i en effektblok som i dette eksempel:

```ruby
with_fx :reverb do
  sample :guit_e_fifths
end
```

- Du kan også tilføje effekter ovenpå andre effekter:

```ruby
with_fx :reverb do
  with_fx :distortion do
    sample :guit_e_fifths
  end
end
```

- Leg lidt med nogle effekter og tilføj dem til din musik. Husk at en fuld liste af effekter kan findes i hjælpedokumentet af Sonic Pi under **FX**.
