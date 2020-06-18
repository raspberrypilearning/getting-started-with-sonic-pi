## Verwende Samples (Beispiele)

Du kannst Musik in Sonic Pi nicht nur mit einzelnen Noten erstellen, sondern auch mit Samples. Samples sind vorab aufgenommene Sounds oder Musikstücke, die du in deine Musik einfügen kannst. Dies ist eine wirklich einfache Methode, um deine Musik erstaunlich klingen zu lassen!

Um ein Sample zu verwenden, musst du den Code `sample :Name des Samples` in der Sequenz deines Musikprogramms einfügen, wo du es abspielen möchtest.

In diesem Beispiel ist `loop_amen` der Name des Samples:

```ruby
2.times do
  sample :loop_amen
  sleep 1.753
end
```

### Samples zum Ausprobieren

Sonic Pi enthält viele Samples. Um deren Namen zu finden, klicke auf **help** gefolgt von **samples** auf der linken Seite des Hilfefensters. Klicke auf einen der Beispielnamen, um weitere Informationen zur Verwendung zu erhalten.