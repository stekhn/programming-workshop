# Textmanipulation

Mit Zeichenketten (*strings*) zu arbeiten gehört zum Alltag eines jeden Programmierers. JavaScript bietet dafür viele nützliche Methoden:

Strings verketten:

```javascript
const name = 'Philipp';
const age = 25;
const occupation = 'Koch';
const city = 'Stuttgart';

// Modernes JavaScript
console.log(`${Philipp} ist ${age} Jahre alt und arbeitet als ${occupation} in ${city}`);

// Oldschool JavaScript
console.log(name + ' ist ' + age + ' Jahre alt und arbeitet als ' + occupation + ' in ' + city);
```

Die moderne Methode ist gerade bei mehreren Variablen deutlich einfach zu schreiben und vermeidet Fehler durch fehlende `+`-Zeichen und Leerzeichen.

Länge eines Textstrings ermitteln:

```javascript
const name = 'Philipp';
console.log(name.length);

// 7
```

Jede String ist für JavaScript ein Array and Buchstaben und Zeichen und hat daher auch eine Länge. Auf die einzelnen Werte kann über den Index (die Position im Array) auch direkt zugegriffen werden:

```javascript
const name = 'Philipp';
console.log(name[1]);

// h
```

Um einen Zeichenkombination in eine String zu finden, können wir die Array-Methode `Array.indexOf()` verwenden:

```javascript
const phrase = 'Philipp ist cool';
console.log(phrase.indexOf('ist'));

// 8
```

Das Wort `ist` finde wir an achter Stelle im Array. Wir eine Zeichenkombination nicht gefunden, gibt die Methode immer `-1` zurück. Das ist nützlich um zum Beispiel zu überprüfen ob ein bestimmter Wert in einer Liste (Array) an Werten vorkommt oder nicht:

```javascript
const participants = ['Philipp', 'Andrea', 'Sophie'];

if (participants.indexOf('Jana') === -1) {
  console.log('Sorry, du stehst nicht auf unserer Liste');
}
```

String in Klein- oder Großbuchstaben umwandeln:

```javascript
const name = 'Philipp';
console.log(name.toLowerCase()); // philipp
console.log(name.toUpperCase()); // PHILIPP
```

Das kann nützlich sein, um Benutzereingaben zu vereinheitlichen, zum Beispiel um daraus Benutzernamen zu generieren oder sie in einer Datenbank zu speichern.

Zeichen in einer Zeichenfolge ersetzt:

```javascript
const phrase = 'Philipp ist cool';
console.log(phrase.replace('Philipp', 'Jana'));

// Jana ist cool
```

⚠️ *Wenn man mit Strings arbeitet, ersetzt `Array.replace()` immer nur den ersten Treffer. Wenn man mehrer Vorkommen eines Strings ersetzen möchte, muss man dazu eine sogenannte [Regular Expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp) verwenden: `phrase.replace(/Philipp/g, 'Jana')`

📖 **MDN**: [Useful string methods](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Useful_string_methods)
