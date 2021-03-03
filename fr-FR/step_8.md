## Jouer deux musiques en même temps

La musique a souvent une piste d'accompagnement répétitive, avec une mélodie distincte jouée sur le dessus. Pour le moment, Sonic Pi a joué une seule musique. Essayons de jouer deux morceaux en même temps !

- Clique sur un nouvel onglet tampon.

2. Le code que nous utilisons pour jouer deux musiques en même temps doit être entre `in_thread do` et `end`.

3. En dessous de `in_thread do`, tape ta musique. Ici, j'ai utilisé un échantillon pour ma piste d'accompagnement :
    
    ```ruby
    in_thread do
      loop do
        sample :loop_amen
        sleep 1.753
      end
    end       
    ```
    
    Ce premier « thread » sera la mélodie de ta musique. En dessous, tu peux taper le code de ta piste d'accompagnement ou de ta ligne de base.

4. Tape :
    
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

5. Maintenant appuie sur **play** et tu devrais entendre les deux threads jouer en même temps.