# Spiel: Rate die Zahl!

### Welche Schritte sind notwendig, um das Spiel umzusetzen?

- Erzeuge eine Zufallszahl zwischen 1 und 100.
- Notiere die Zugnummer, auf der sich der Spieler befindet. Beginne mit 1.
- Gib dem Spieler die Möglichkeit, die Nummer zu erraten.
- Sobald der Benutzer eine Schätzung eingibt, muss diese gespeichert werden, damit der Benutzer seine vorherigen Schätzungen sehen kann.
- Prüfe, ob es sich um die richtige Nummer handelt.
- Wenn die Schätzungen richtig ist:
  - Glückwunschmeldung anzeigen.
  - Spieler davon abhalten, weitere Schätzungen einzugeben.
  - Button anzeigen mit dem der Spieler das Spiel neu starten kann.
- Wenn es falsch ist und der Spieler nach Spielzüge übrig hat:
  - Sag dem Spieler, dass er falsch liegt.
  - Erlaube ihnen, eine weitere Schätzung einzugeben.
  - Erhöhe die Zugnummer um 1.
- Wenn es falsch ist und der Spieler keine Züge mehr hat:
  - Sag dem Spieler, dass das Spiel vorbei ist.
  - Spieler davon abhalten, weitere Schätzungen einzugeben.
  - Button anzeigen mit dem der Spieler das Spiel neu starten kann.
- (Spiel zurücksetzen)

Quelle: https://developer.mozilla.org/de/docs/Learn/JavaScript/First_steps/A_first_splash
