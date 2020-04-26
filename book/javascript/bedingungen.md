### Bedingungen

Mit Bedingungen (*conditionals*) kann man den Ablauf eines Programms steuern. Das Konzept ist relativ leicht zu verstehen, da es sich um eine einfache „Wenn, dann, ansonsten“-Logik handelt.

```javascript
const isHungry = true;

if (isHungry) {
  console.log('Geh was essen!');
} else {
  console.log('Mach deine Hausaufgaben!');
}

// Geh was essen!
```

Wenn die Bedingung `isHungry` wahr, also `true` ist, wird der erste Block ausgeführt. Beim ersten Treffer wird die Schleife abgebrochen. Wenn keine Bedingung zutrifft, wird der `else`-Block ausgeführt werden. Der `else`-Block ist jedoch optional und kann auch weggelassen werden. In diesem Fall würde einfach nichts passieren, beziehungsweise ausgegeben werden.

Man kann auch mehrere Bedingungen definieren:

```javascript
const isHungry = false;
const isThirsty = true;

if (isHungry) {
  console.log('Geh was essen!');
} else if (isThirsty) {
  console('Du solltest was trinken!')
} else {
  console.log('Mach deine Hausaufgaben!');
}

// Du solltest was trinken!
```

In diesem Fall würde der zweite Block `else if`-Block ausgeführt werden.

```javascript
const isHungry = true;
const isThirsty = true;

if (isHungry) {
  console.log('Geh was essen!');
} else if (isThirsty) {
  console('Du solltest was trinken!')
} else {
  console.log('Mach deine Hausaufgaben!');
}

// Geh was essen!
```

Wenn beide Bedingungen wahr sind, würde nur die erste davon ausgegeben werden, da die Schleife abbricht sobald eine Bedingung erfüllt ist. 

```javascript
const isHungry = false;
const isThirsty = false;

if (isHungry) {
  console.log('Geh was essen!');
} else if (isThirsty) {
  console('Du solltest was trinken!')
} else {
  console.log('Mach deine Hausaufgaben!');
}

// Mach deine Hausaufgaben!
```

Wenn keine Bedingung erfüllt wird, tritt der `else`-Fall ein.

Man kann in den Bedingungen auch mit logischen Operatoren arbeiten. Wichtig ist aber, dass diese irgendeinen Wahrheitswert zurückgeben. In diesem Beispiel ist auch die Reihenfolge der Bedingungen wichtig, da diese logisch aufeinander aufbauen.

In diesem Beispiel bauen wir einen Empfehlungsalgorithmus, der bestimmt wann ein Kind zuhause sein muss:

```javascript
const age = 15;

if (age > 18) {
  console.log('Sei bitte bis spätestens 2 Uhr zuhause!');
} else if (age > 16) {
  console.log('Sei bitte bis spätestens 24 Uhr zuhause!');
} else if (age > 14) {
  console.log('Sei bitte bis spätestens 22 Uhr zuhause!');
} else if (age > 12) {
  console.log('Sei bitte bis spätestens 20 Uhr zuhause!');
} else {
  console.log('Wenn du älter bist, darfst du auch mal aus dem Haus.');
}

// Sei bitte bis spätestens 22 Uhr zuhause!
```

Außerdem kann man Bedingungen ineinander verschachteln. In diesem Fall darf ein Kind länger wegbleiben, wenn eine volljährige Aufsichtsperson mit dabei ist. Es sei denn, dass Kind ist 14 oder jünger, dann muss es um 22 Uhr zuhause sein.  

```javascript
const hasChaperone = true;
const age = 15;

if (hasChaperone) {
  if (age <= 14 ) {
    console.log('Sei bitte bis spätestens 22 Uhr zuhause!')
  } else {
    console.log('Egal wann du nach Hause kommst, aber benimm dich!')
  }
} else {
  if (age >= 18) {
    console.log('Sei bitte bis spätestens 2 Uhr zuhause!');
  } else if (age >= 16) {
    console.log('Sei bitte bis spätestens 24 Uhr zuhause!');
  } else if (age >= 14) {
    console.log('Sei bitte bis spätestens 22 Uhr zuhause!');
  } else if (age >= 12) {
    console.log('Sei bitte bis spätestens 20 Uhr zuhause!');
  } else {
    console.log('Wenn du älter bist, darfst du auch mal aus dem Haus.');
  }
} 

// Sei bitte bis spätestens 22 Uhr zuhause!
```

💡 *Man sollte es mit dem Verschachteln von if-Bedingungen nicht übertreiben. Mehr als drei Logik-Ebenen sind schwer zu verstehen, führen zu endlosen Fehlersuchen und werden generell als schlechten Stil angesehen.*

⚠️ *Wenn man eine definierte Variable, Konstante oder Funktion als Bedingungen angibt, ist diese immer `true`. Die kann man dazu nutzen, um zu überprüfen ob Benutzereingaben stimmen. Allerdings ist diese Verhalten auch ein häufige Fehlerquelle. Am besten prüft man immer explizit, ob ein Wert definiert ist: `if (userName !== undefined)`*

📖 **MDN**: [Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)
