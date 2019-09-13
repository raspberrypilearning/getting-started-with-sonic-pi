## Adăugarea de efecte

Sintetizatoarele moderne au capacitatea de a adăuga efecte la sunete. Sonic Pi nu este diferit: poți adăuga efecte de studio, cum ar fi reverb, ecou și distorsiuni. Desigur, trebuie să scrii cod pentru a adăuga efectele!

- Într-o foaie de lucru nouă găsește un eșantion cate îți place, de exemplu `sample :guit_e_fifths`

- Introdu eșantionul într-un bloc de efecte astfel:
    
    ```ruby
    with_fx :reverb do
      sample :guit_e_fifths
    end
    ```

- Poți adăuga un nou efect peste cel existent astfel:
    
    ```ruby
    with_fx :reverb do
      with_fx :distortion do
        sample :guit_e_fifths
      end  
    end
    ```

- Joacă-te cu niște efecte și adaugă-le la muzica ta. Ține minte că o listă completă a efectelor poate fi găsită în secțiunea de ajutor a Sonic Pi sub **FX**.