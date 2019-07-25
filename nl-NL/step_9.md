## Live coderen!

Sonic Pi is ontwikkeld als een platform voor het live coderen van muziek, zodat de code in realtime kan worden gemanipuleerd, gewijzigd en aangepast; dit betekent dat programmeurs hun code kunnen uitvoeren in plaats van vooraf geschreven programma's te spelen. Waarom probeer je het niet?

- In een nieuwe buffer tab typ je:
    
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

- Druk op **Run** om het programma te starten.

- Terwijl de melodie speelt, schakel je de laatste drie regels uit door een `#` symbool toe te voegen aan het begin van elke regel, zoals hier:
    
    ```ruby
    # loop do
    #   play_my_synth
    # end
    ```

- Wijzig vervolgens een deel van de code in de functie en druk nogmaals op **Run**. Nu ben je echt aan het rocken!