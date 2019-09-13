## Repetă o melodie

Acum stăpânești elementele de bază ale Sonic Pi, să scriem cod pentru o melodie!

- Selectează **Buffer 2**.

2. Tastează următorul cod:
    
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

3. Acum dă click pe pictograma de redare din partea de sus a ecranului și va fi redată prima parte a unei melodii. Poți spune ce melodie este?
    
    *Răspuns: Frère Jacques!*
    
    Această primă secțiune trebuie redată de două ori. Cum ai putea să o repeți? Ai putea introduce aceeași secțiune din nou, sau am putea începe să introducem bucle în codul tău.

4. În partea de sus a codului tău, deasupra primei linii `play 60`, scrie:
    
    ```ruby
    2.times do
    ```

5. Iar în partea de jos a codului, sub `sleep 0.5`, scrie:
    
    ```ruby
    end
    ```

6. Dă click pe pictograma de redare din partea de sus a ecranului. Ce se întâmplă?
    
    Să redăm bucata asta în Sonic Pi.
    
    În exemplul de mai jos, poți vedea că unele linii de cod sunt indentate. Acest lucru ușurează citirea codului și verificarea eventualelor erori în cazul în care nu funcționează atunci când apeși butonul de redare. Poți apăsa de două ori bara de spațiu pentru a indenta linia de cod.
    
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

### Repetă la infinit?

Repetarea notelor de un anumit număr de ori este cu siguranță utilă, dar ce se întâmplă dacă dorești să repeți melodia la infinit?

În loc să folosești `2.times do` și `end` poți scrie `loop do` și `end`, astfel:

```ruby
loop do
  play 60
  sleep 0.5
end
```