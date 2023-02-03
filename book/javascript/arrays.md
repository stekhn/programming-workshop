# Arrays

Arrays sind die einfachste Möglichkeit um Listen in JavaScript zu erstellen. Diese Listen können beliebige Informationen erhalten. Neben Zeichen, Zahlen und Wahrheitswerten können Arrays auch weitere Arrays oder Objekte enthalten.

Hier ein Beispiel für ein einfaches Array mit drei Namen:

```javascript
const names = ["Philipp", "Andrea", "Sophie"];
```

Die einzelnen Einträge in einem Array kann man über ihren Stellenwert (_Index_) abfragen:

```javascript
const names = ["Philipp", "Andrea", "Sophie"];

console.log(names[0]);
// Philipp
console.log(names[1]);
// Andrea
console.log(names[2]);
// Sophie
```

> 💡 _In den meiste Programmiersprachen ist das erste Element eines Arrays immer das nullte Element. Das ist auch insofern verwirrend, da die Länge eines Elements normal gezählt wird. Hat ein Array fünf Elemente, ist das letzte Element das vierte Element, die Länge des Arrays `array.length` ist aber trotzdem Fünf. Um auf das letzte Element zuzugreifen, kann man sich das zunutze machen und `array[array.length - 1]` schreiben._

Um einem Array neue Elemente hinzuzufügen, kann man die Methode **Array.push()** verwenden:

```javascript
const names = ["Philipp", "Andrea", "Sophie"];

names.push("Yusuf");
console.log(names);
// ['Philipp', 'Andrea', 'Sophie', 'Yusuf']
```

**Array.reverse()** dreht die Reihenfolge der Element in einem Arrays um:

```javascript
const names = ["Philipp", "Andrea", "Sophie"];

names.reverse();
console.log(names);
// ['Sophie', 'Andrea', 'Philipp']
```

Mit der Methode **Array.sort()** ein Array sortieren:

```javascript
const names = ["Philipp", "Andrea", "Sophie"];

names.sort();
console.log(names);
// ['Andrea', 'Philipp', 'Sophie']
```

Allerdings sortiert JavaScript die Werte eines Arrays lexikalisch. Daher braucht man eine extra Funktion, um Zahlenwerte aufsteigend sortieren zu können:

```javascript
const numbers = [5, 12, 8, 130, 11, 44];

numbers.sort();
console.log(numbers);
// [11, 12, 130, 44, 5, 8]

numbers.sort((a, b) => a - b);
console.log(numbers);
// [5, 8, 11, 12, 44, 130]
```

Man kann Arrays mit **Array.find()** auch nach bestimmten Bedingungen durchsuchen. In diesem Beispiel wollen wir alle Zahlen finden, welche größer als 10 sind:

```javascript
const numbers = [5, 12, 8, 130, 11, 44];
const found = numbers.find((n) => n > 10);

console.log(found);
// [12, 11]
```

Es gibt noch unzählige weitere Methoden, um mit Arrays zu arbeiten. Arrays können beispielsweise geteilte, mit anderen Arrays verbunden oder in Text umgewandelt werden. Besonders wichtig ist die Methode **Array.forEach()** welche im Kapitel Schleifen besser beschrieben wird.

📖 **MDN**: [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
