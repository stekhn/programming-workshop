### Funktionen

Funktionen sind eine sinnvolle Möglichkeit JavaScript-Programme zu strukturieren und wiederverwendebare Code-Schnipsel zu definieren. Hier die wichtigsten Eigenschaften:

- Funktionen sind Unterprogramme, welche bestimmte Aufgabe erfüllen.
- Funktionen werden erst dann ausgeführt, wenn sie aufgerufen werden.
- Werte können als Parameter an die Funktion übergeben und innerhalb der Funktion als Argumente verwendet werden.
- Funktionen geben immer Wert zurück. Wenn eine Funktion kein `return`-Statement hat, wird immer `undefined` zurückgegeben.

Es gibt verschiedene Möglichkeiten, eine Funktion in JavaScript zu definieren:

Eine Funktionsdeklaration definiert eine benannte Funktion. Um eine Funktionsdeklaration zu erstellen, verwenden Sie das functionSchlüsselwort gefolgt vom Namen der Funktion. Beim Verabeiten des JavaScript-Codes werden Funktionsdeklaration immer an den Anfang des Codes gesetzt, sodass die Funktion verwendet werden kann, bevor sie definiert wurde.

```javascript
// Funktion kann verwenden werden, bevor sie definiert wurde
sayHello('Philipp');

function sayHello(name)  {
  console.log('Hallo ' + name);
};
```

Ein Funktionsausdruck definiert eine benannte oder anonyme Funktion. Eine anonyme Funktion ist eine Funktion die keinen Namen hat. Funktionsausdrücke können erst verwendet werden, nach dem sie definiert wurden:

```javascript
const sayHello = function (name)  {
  console.log('Hallo ' + name);
};

// Funktion kann erst verwendet werden, nach dem sie definiert wurde
sayHello('Philipp');
```

Ein Pfeilfunktionsausdruck ist eine kürzere Syntax zum Schreiben von Funktionsausdrücken. Pfeilfunktionen erzeugen keinen eigenen `this`-Wert.

```javascript
const sayHello = (name) => {
  console.log('Hallo ' + name);
};

// Funktion kann erst verwendet werden, nach dem sie definiert wurde
sayHello('Philipp');
```

📖 **MDN**: [Functions](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Functions)   
📖 **Codeburst**: [JavaScript Functions](https://codeburst.io/javascript-functions-understanding-the-basics-207dbf42ed99)
