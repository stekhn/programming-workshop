# Schleifen

Schleifen (*loops*) sind nützlich, um sich wiederholende Aufgaben innerhalb eines Programms schnell zu erledigen. In JavaScript gibt es verschieden Möglichkeiten Schleifen zu programmieren. Jede Möglichkeit hat bestimmte Vor- und Nachteile.

**For-Schleifen** sind die flexibelsten Formen von Schleifen und bestehen aus `for(Zähler, Abbruchbedingung, Iterator)`. Der Zähler `i` definiert eine Variable und ihren Startwert (meistens Null). Die Abbruchbedingung definiert, wann die Schleife zu Ende sein soll – in diesem Beispiel bevor der Zähler den gleichen Wert hat, wie die Anzahl der Personen (`names.length`). Der Iterator legt den Betrag fest, um den der Zähler `i` erhöht (oder erniedrigt) wird. `i++` bedeutet in diesem Fall, dass der Zähler immer um eins erhöht wird.

```javascript
const names = ['Philipp', 'Andrea', 'Sophie'];

for (let i = 0; i < names.length; i++) {
  console.log(`Hallo ${names[i]}, du bist die Nummer ${i}`);
}

// Hallo Philipp, du bist die Nummer 0
// Hallo Philipp, du bist die Nummer 1
// Hallo Philipp, du bist die Nummer 2
```

Direkt auf den Zähler zugreifen zu können ist dann praktisch, wenn man zum Beispiel nur jede zweite Person ausgeben möchte `i += 2`, kurz für `i = i + 2`. Wichtig ist, dass die Abbruchbedingung erreicht werden kann, da die Schleife sonst endlos läuft und das Programm oder der Browser abstürzen kann. Die folgenden Möglichkeiten eine Schleife zu schreiben sind  deutlich sicherer:

**For-Of-Loops** für Arrays kann man dann verwenden, wenn man nicht auf einen Zähler angewiesen ist:

```javascript
const names = ['Philipp', 'Andrea', 'Sophie'];

for (let name of names) {
  console.log(`Hallo ${name}.`);
}
```

**For-In-Loops** für Objekte funktioniert ganz ähnlich, werden aber eher selten verwendet:

```javascript
const names = {
  personA: 'Philipp',
  personB: 'Andrea',
  personC: 'Sophie'
};

for (let name in names) {
  console.log(`Hallo ${name}.`);
}
```

**Array.forEach()** ist eine weitere Funktion mit der man über Arrays iterieren (Nerd-Sprech für Schleifen bauen) kann. Der Vorteil ist, dass man hier auch auf den Index (Position im Array) eines Wertes zugreifen kann:

```javascript
const names = ['Philipp', 'Andrea', 'Sophie'];

names.forEach((name, index) => {
  console.log(`Hallo ${name}, du bist die Nummer ${index}.`);
});
```

Vergleichbare Schleifen kann man mit den Funktionen **Array.map()** oder **Array.reduce()** bauen, welche genutzt werden können, um die Daten eines Arrays entweder zu verändern oder zusammenzufassen. Außerdem gibt es noch **While-Schleifen** und **Do-While-Schleifen**, die aber keinen Vorteil gegenüber der normalen **For-Loop** bieten und ein wenig „oldschool“ sind.

📖 **MDN**: [Looping code](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code)  
📖 **Impressive Webs**: [What’s the Best Way to Write a JavaScript For Loop?](https://www.impressivewebs.com/javascript-for-loop/)
