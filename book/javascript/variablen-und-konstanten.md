### Variablen und Konstanten

Variablen `let` und Konstanten `const` sind notwendig um Werte zu speichern und später wieder aufzurufen. Diese Konzept gibt es in eigentlich jeder Programmiersprache.  

Variablen können, nach dem sie erstellt (deklariert wurde), mit einem anderen Wert überschrieben werden.

```javascript
// Deklaration der Variable
let name = 'Philipp';

// Kann überschrieben werden
name = 'Marlene';
```

Konstanten können, wie der Name andeutet, nicht überschrieben werden:

```javascript
// Deklaration der Konstanten
const name = 'Philipp';

// Kann nicht überschrieben werden und führt zu einem Fehler:
// Uncaught TypeError: Assignment to constant variable.
name = 'Marlene';
```

In altem JavaScript-Code findet man oft noch `var`-Variablen. Diese funktionieren relativ ähnlich wie `let`-Variablen, sollten aber nicht mehr verwendet werden. Wo möglich immer `const` verwenden, für alles andere `let`.
