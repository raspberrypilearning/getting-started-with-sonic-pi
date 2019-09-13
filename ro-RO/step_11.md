## Modificarea parametrilor

În unele ocazii, ți-ai putea dori să faci sunetele să dureze mai mult timp sau să fie redate la o frecvență diferită. Acest lucru poate fi realizat cu ușurință prin modificarea parametrilor codului pe care îl folosești.

Să luăm `play 60`, de exemplu.

- Dă click pe **help** pentru a deschide documentația, apoi selectează **lang** în partea stângă, și derulează până la **play**. Vei vedea câteva exemple de utilizare. Până acum ai folosit `play` fără parametri; să folosim câțiva acum.
- Într-o de foaie de lucru nouă scrie:
    
    ```ruby
    play 60, attack: 1, release: 3
    ```

- Apasă pe butonul **play** pentru a afla cum se aude acea notă. Atacul și release-ul controlează amplitudinea unei note în timp.

- Acum schimbă valorile pentru atac și release pentru a vedea cum acești parametri afectează nota.

Există o mulțime de parametri care pot schimba, de asemenea, modul în care sună eșantioanele sau sintetizatoarele. Încearcă să modifici valorile pentru `cutoff:`, `pan:`, `rate:` sau `amp:`.

Pentru o listă completă a parametrilor pentru fiecare eșantion, dă click pe pictograma **Help**, apoi pe **Samples**. Selectează un eșantion și derulează în jos pentru a vedea o explicație completă pentru fiecare tip de parametru care poate fi utilizat cu acesta. Același lucru este valabil și pentru sintetizatoare!