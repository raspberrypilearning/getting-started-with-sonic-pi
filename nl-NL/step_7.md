## Gebruik samples

Je kunt niet alleen muziek maken in Sonic Pi met losse noten, je kunt ook muziek maken met samples. Samples zijn vooraf opgenomen geluiden of melodieën die je in jouw muziek kunt gebruiken. Dit is een heel eenvoudige manier om je muziek geweldig te laten klinken!

Om een ​​sample te gebruiken, moet je de code `sample: naam van sample` toevoegen de regels code van je muziekprogramma waar je het wilt afspelen.

In dit voorbeeld is `loop_amen` de naam van de sample:

```ruby
2.times do
  sample :loop_amen
  sleep 1.753
end
```

### Samples om te proberen

Er zijn veel samples opgenomen in Sonic Pi. Om de namen ervan te vinden, klik je op **Help** gevolgd door **Samples** onder het helpvenster. Klik op een van de samplenamen voor meer informatie over het gebruik ervan.