## Utilizarea rrand

Sonic Pi include o serie de funcții care pot adăuga mai multe elemente interesante muzicii tale. O funcție foarte distractivă este `rrand`, care va returna o valoare aleatoare între două numere specificate. Pentru un efect interesant, folosește `rrand` pentru a face parametrul cutoff să varieze.

- Într-o foaie de lucru nouă scrie:
    
    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: 80
      sleep 0.2
    end
    ```

- În loc de a trece un număr ca `80` la valoarea de cutoff, încearcă `rrand (40, 120)`, pentru a obține un număr aleator între 40 și 120, astfel:
    
    ```ruby
    loop do
      play chord(:a3, :minor).choose, attack: 0, release: 0.3, cutoff: rrand(40, 120)
      sleep 0.2
    end
    ```

- Apoi poți începe să experimentezi folosind `rrand` cu alți parametri. De exemplu, adaugă `pan: rrand (-1, 1)` la linia play chord și apoi apasă **play**.