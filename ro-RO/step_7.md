## Utilizează eșantioane

Nu numai că poți crea muzică în Sonic Pi utilizând note individuale, dar poți crea muzică și cu eșantioane. Eșantioanele sunt sunete sau melodii preînregistrate pe care le poți insera în muzica ta. Aceasta este o modalitate foarte simplă de a face muzica ta să sune nemaipomenit!

Pentru a utiliza un eșantion, trebuie să adaugi `sample :nume_eșantion` în programul tău acolo unde vrei să fie redat.

În acest exemplu, `loop_amen` este numele eșantionului:

```ruby
2.times do
  sample :loop_amen
  sleep 1.753
end
```

### Eșantioane de încercat

Există o mulțime de eșantioane incluse în Sonic Pi. Pentru a găsi numele acestora, dă click pe **help** apoi pe **samples** în partea stângă a ferestrei de ajutor. Dă click pe numele oricăruia dintre eșantioane pentru a obține mai multe informații despre cum să îl folosești.