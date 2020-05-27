# JavaScript-Aufgaben

Hier ein paar Aufgaben, um deine JavaScript-Fähigkeiten zu testen.

## Funktionen

Schreibe eine Funktion, welche das Volumen eines Quaders (Länge x Breite x Höhe) berechnet

```javascript
function calculateVolume(a, b, c) {

  if (a < 0 || b < 0 || c < 0) {
    console.error('Alle Eingabenwerte müssen größer als Null sein.')
  } else {
    return a * b * c;
  }
}

calculateVolume(35, 20, 70) // => 49000
```

*Profi-Frage:* Angenommen man hat eine Funktion `calculateArea`, mit der man die Fläche eines Rechtecks berechnen kann. Die Funktion akzeptiert aber nur zwei Parameter. Könnte man diese Funktion – ohne sie zu verändern – trotzdem nutzen, um damit das Volumen eines Quaders zu berechnen?

```javascript
function calculateArea(a, b) {
  return a * b;
}

const volume = calculateArea(calculateArea(20, 20), 20);
console.log(volume) // => 8000
```

## Bedingungen

Schreibe eine Funktion die abhängig von der aktuellen Uhrzeit entweder „Guten Morgen“, „Guten Tag“, „Guten Abend“ oder „Gute Nacht“ ausgibt:

```javascript
function sayHelloByTime() {
  const hour = new Date().getHours();

  if (hour >= 6 && hour < 12) {
    console.log('Guten Morgen');
  }

  if (hour >= 12 && hour < 16) {
    console.log('Guten Tag');
  }

  if (hour >= 16 && hour < 22) {
    console.log('Guten Abend');
  }

  if (hour >= 22 && hour < 4) {
    console.log('Gute Nacht');
  }
}

sayHelloByTime() // => Guten Tag
```

## Schleifen

Wir haben ein Array mit verschieden Zahlen. Schreibe eine Funktion, welche alle Zahlen addiert und die Summe ausgibt.

```javascript
const numbers = [12, 412, 52, 68, 21, 546];

function sumAll(array) {
  let sum = 0;

  array.forEach(function (number) {
    sum = sum + number;
  });

  console.log(sum);
  return sum;
}

sumAll(numbers) // => 1111
```

Alternativ kann man auch die Funktion `Array.reduce()` verwenden:

```javascript
const numbers = [12, 412, 52, 68, 21, 546];

function sumAll(array) {
  const sum = array.reduce(function (accumulator, current) {
    return accumulator + current;
  }, 0);

  console.log(sum);
  return sum;
}

sumAll(numbers) // => 1111
```

## Schleifen und Bedingungen

Wir haben ein Array mit verschieden geraden und ungeraden Zahlen. Schreibe eine Funktion, welche nur die geraden Zahlen addiert und die Summe ausgibt.

```javascript
const numbers = [617, 122, 31, 168, 76, 71, 129, 300]

function sumEven(array) {
  let sum = 0;

  array.forEach(function (number) {
    if (number % 2 === 0) {
      sum = sum + number;
    }
  });

  console.log(sum);
  return sum;
}

sumEven(numbers) // => 666
```

## Arrays

Wir haben ein Array mit verschiedenen Namen. Deine Aufgabe ist es, eine Funktion zu schreiben, welche alle Personen einzeln begrüßt.

```javascript
const names = ['Philipp', 'Andrea', 'Sophie'];

function sayHello(array) {
  for (var i = 0; i < array.length; i++) {
    console.log(`Hallo ${names[i]}. `);
  }
}

sayHello(names); // => Hallo Philipp. Hallo Andrea. Hallo Sophie.
```

## Objekte

Objekte sind neben Arrays eine andere Möglichkeit digitale Listen zu führen. In diesem Beispiel wollen wir Philipps Alter wissen:

```javascript
const person = { name: 'Philipp', age: 31 };

function getAge(object) {
  console.log(`${object[name]} ist ${object.age} Jahre alt.`);
}

getAge(person); // => Philipp ist 31 Jahre alt.
```

## Object-Arrays

Arrays bestehen nicht immer nur aus Buchstaben oder Zahlen, sondern manchmal auch aus mehreren Objekten. Das ist praktisch, um zum Beispiel Personen mit mehreren Eigenschaften zu speichern. Schaffst du es, alle Personen mit ihrem Namen und Herkunftsort zu begrüßen?

```javascript
const persons = [
  { name: 'Philipp', city: 'Stuttgart' },
  { name: 'Andrea', city: 'Hamburg' },
  { name: 'Sophie', city: 'Dresden' }
];

function sayHelloCity(objectArray) {
  let string = '';

  for (const i in objectArray) {
    string += `Hallo ${objectArray[i].name} aus ${objectArray[i].city}. `;
  }

  console.log(string);
}

sayHelloCity(persons); // => Hallo Philipp aus Stuttgart. Hallo Andrea aus Hamburg. Hallo Sophie aus Dresden.
```
