## Redarea a două melodii în același timp

Muzica are adesea o pistă de acompaniament care se reperă, cu o melodie separată interpretată peste aceasta. Până acum, în Sonic Pi ai redat o singură melodie. Să încercăm să redăm două melodii în același timp!

- Dă click pe un tab new buffer.

2. Codul pe care îl folosim pentru a reda două melodii în același timp trebuie să fie între `in_thread do` și `end`.

3. Sub `in_thread do`, introdu melodia ta. Aici am folosit un eșantion pentru pista de acompaniament:
    
    ```ruby
    in_thread do
      loop do
        sample :loop_amen
        sleep 1.753
      end
    end       
    ```
    
    Primul „fir de execuție” (thread) va conține melodia ta. În partea de jos, poți introduce codul pentru pista de acompaniament.

4. Scrie:
    
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

5. Acum, apasă tasta **play** și ar trebui să auzi ambele sunete care sunt redate în același timp.