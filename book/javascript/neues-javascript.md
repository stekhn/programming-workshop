# Neues JavaScript

In den letzten Jahren hat sich JavaScript als Sprache stark weiterentwickelt. Das hat auch einige Veränderungen in der Syntax mit sich geführt, so dass neueres JavaScript ein wenig anders aussieht als altes JavaScript

**Altes JavaScript** (auch ECMAScript 5 oder auch ES5)

```javascript
var names = ["Philipp", "Andrea", "Sophie"];

var sayHello = function (array) {
  for (var i = 0; i < array.length; i++) {
    console.log("Hallo " + array[i] + ".");
  }
};

sayHello(names);
```

**Neues JavaScript** (auch ECMAScript 6, ES6, ES2015, ES2016, ES2017 ...):

```javascript
const names = ["Philipp", "Andrea", "Sophie"];

const sayHello = (array) => {
  for (let i = 0; i < array.length; i++) {
    console.log(`Hallo ${array[i]}.`);
  }
};

sayHello(names);
```

Da noch nicht alle Browser das neue JavaScript perfekt beherrschen, braucht man so genannte _Transpiler_ die zwischen den unterschiedlichen JavaScript-Version hin und her übersetzen können. Der bekannteste Transpiler um neues JavaScript in altes JavaScript zu übersetzen ist [Babel](https://babeljs.io/repl). Um altes JavaScript in neues JavaScript zu übersetzen gibt es [Lebab](https://lebab.unibtc.me/editor) (Babel rückwärts geschrieben).

💡 _Am einfachsten lässt sich neues JavaScript an den Variablennamen `let`, `const` und der Arrow-Funktionen `() => {}` erkennen._

📖 **Ralf S. Engelschall**: [ECMAScript 6 – New Features](http://es6-features.org/)
