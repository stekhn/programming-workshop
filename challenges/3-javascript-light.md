# JavaScript-Aufgaben

Hier ein paar Aufgaben, um deine JavaScript-Fähigkeiten zu testen. Kopiere die jeweiligen Code-Schnipsel in einem HTML-Script-Element und vervollständige sie. Die Ergebnisse deiner Berechnungen kannst mit `console.log(result)` in die Konsole der Chrome Entwicklerwerkzeuge schreiben.

## Objekte

Objekte sind neben Arrays eine andere Möglichkeit digitale Listen zu führen. In diesem Beispiel wollen wir Philipps Alter wissen:

```javascript
const person = { name: 'Philipp', age: 31 };

// Dein Code hier ...

console.log(result);
// => Philipp ist 31 Jahre alt.
```

**Tipp:** eigener Text und Variablen kannst du mit dem `+`-Symbol verketten. Beispiel: `console.log('Hallo' + person.name)`

## Object-Arrays

Arrays bestehen nicht immer nur aus Buchstaben oder Zahlen, sondern manchmal auch aus mehreren Objekten. Das ist praktisch, um zum Beispiel Personen mit mehreren Eigenschaften zu speichern. Schaffst du es, alle Personen mit ihrem Namen und Herkunftsort zu begrüßen?

```javascript
const persons = [
  { name: 'Philipp', city: 'Stuttgart' },
  { name: 'Andrea', city: 'Hamburg' },
  { name: 'Sophie', city: 'Dresden' }
];

// Dein Code hier ...

console.log(result);
// => Hallo Philipp aus Stuttgart. Hallo Andrea aus Hamburg. Hallo Sophie aus Dresden.
```

**Tipp:** Zum Lösen der Aufgabe kannst du eine `forEach`-Schleife verwenden. Um Text an einen bestehendende Variable (z.B. `result`) anzuhängen, kannst du das `+=`-Symbol verwenden.

**Bonus:**: Andrea grüßt nie zurück, deswegen wollen wir sie auch nicht mehr grüßen. Stelle also sicher, dass Menschen mit dem Namen Andrea nicht gegrüßt werden. Nie wieder.
