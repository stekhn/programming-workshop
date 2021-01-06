# Objekte

Objekte sind ähnliche wie Arrays (Listen) eine weitere Methode um Daten in JavaScript zusammenzuhalten. Im Gegensatz zu Arrays können die einzelnen Eigenschaften (*properties* oder *keys*) eines Objekts aber benannt werden.

```javascript
const person = {
  name: 'Philipp',
  age: 23,
  city: 'Hamburg'
};
```

Die einzelnen Werte in einem Objekt kann man über den jeweiligen Namen mit der sogenannten Punktnotation (*dot notation*) abfragen:

```javascript
const person = {
  name: 'Philipp',
  age: 23,
  city: 'Hamburg'
};

console.log(person.name);
// Philipp
```

Genauso kann man Objekten relativ einfach neue Eigenschaften hinzufügen:

```javascript
const person = {
  name: 'Philipp',
  age: 23,
  city: 'Hamburg'
};

person.job = 'teacher':

console.log(person)
// {
//   name: 'Philipp',
//   age: 23,
//   city: 'Hamburg',
//   job: 'teacher'
// }
```

Das funktioniert aber nur so lange der Name der Eigenschaft ein Wort ohne Sonderzeichen ist. Kommen Umlaute, Leerzeichen oder Bindestriche im Namen vor, funktioniert die Punktnotation nicht mehr. In diesem Fall benötigen wir die Klammernotation (*bracket notation*). Außerdem müssen wir die Eigenschaft in Anführunszeichen (`'` oder `"`) schreiben:

```javascript
const person = {
  name: 'Philipp',
  age: 23,
  city: 'Hamburg',
  job: 'teacher',
  'last-job': 'bike mechanic'
};

console.log(person['last-job']);
// bike mechanic
```

Der Wert einer Eigenschaft ist nicht nur auf Texte oder Zahlen beschränkt und kann genauso gut auch eine Array oder eine Funktion sein:

```javascript
const person = {
  name: 'Philipp',
  age: 23,
  city: 'Hamburg',
  married: false,
  partner: undefined,
  hobbies: ['reading', 'climbing', 'travelling'],
  sayHello: function () { console.log('Hi, my name is ' + this.name) } 
};

console.log(person.hobbies);
// ['reading', 'climbing', 'travelling']

console.log(person.sayHello());
// Hi, my name is Philipp
```

Relativ häufig sieht man die Verwendung in Verbindung mit Arrays. Um zum Beispiel die Daten eine Gruppe von Menschen zu speichern bietet sich ein sogenanntes *Object Array* an:

```javascript
const persons = [
  {
    name: 'Philipp',
    age: 23,
    city: 'Hamburg'
  };
  {
    name: 'Andrea',
    age: 52,
    city: 'München'
  },
  {
    name: 'Sophie',
    age: 31,
    city: 'Berlin'
  }
];
```

Die Daten dieses *Object Array* lassen sich an einfachsten mit einer Schleife verarbeiten.

📖 **MDN**: [Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)  
📖 **MDN**: [Property accessors](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Property_Accessors)  
📖 **MDN**: [Working with JSON](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON)
