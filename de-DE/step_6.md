## Ändere die Sounds

Es ist an der Zeit, deinen Song interessanter zu machen! Wir können dies tun, indem du die verwendeten Synthesizer-Sounds änderst. Der standardmäßige Sonic Pi-Synth heißt `beep` (auf Deutsch: piepen).

Um einen anderen Synthesizer (kurz synth) zu verwenden, musst du den Code `use_synth: Name des Synthesizer` oberhalb der Code-Reihenfolge einfügen, in der du ihn verwenden möchtest.

In diesem Beispiel ist `fm` der Name des Synth:

```ruby
use_synth :fm
2.times do
  play 60
  sleep 0.5
  play 67
  sleep 0.5
end
```

### Synthesizer zum Ausprobieren

Sonic Pi enthält viele cool klingende Synthesizers. Um deren Namen zu finden, klicke auf das Symbol **help** oben auf dem Bildschirm, um das Fenster mit den Hilfedokumenten anzuzeigen. Wähle dann in den Registerkarten links im Hilfefenster **synths** aus. Klicke auf einen der Synthesizer-Namen, um weitere Informationen zur Verwendung zu erhalten.