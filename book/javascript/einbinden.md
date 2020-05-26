# Einbinden

JavaScript kann auf deiner eigene Seite auf zwei Wegen eingebunden werden. Für kleine Webprojekte kann man den JavaScript-Code direkt in einem `<script>`-Element schreiben:

```html
<!DOCTYPE html>
<html lang="de">
<head>
 <title>Titel der Webseite</title>
</head>
<body>
  <button id="submit">Abschicken</button>
  <script>
    document.querySelector('button#submit').addEventHandler('click', () => {
      console.log('Button wurde geklickt');
    });
  </script>
</body>
</html>
```

Für größere Projekte empfiehlt es sich jedoch den JavaScript-Code in eine eigenen Datei zu schreiben und diese über einen `<script>`-Tag mit `src`-Attribut einzubinden:

```html
<!DOCTYPE html>
<html lang="de">
<head>
  <title>Titel der Webseite</title>
</head>
<body>
  <button id="submit">Abschicken</button>
  <script src="script.js"></script>
</body>
</html>
```

Im Gegensatz zu unserem CSS-Beispiel haben wir die Skripte nicht im `<head>`-Bereich der Seite eingebunden. Das liegt daran, dass unser JavaScript-Code davon abhängt, dass das Element `<button>` schon erstellt wurde. Das ist jedoch nur sichergestellt, wenn wir unseren JavaScript-Code in der Dokumentenstruktur (DOM) erst nach dem oder den benötigeten Elementen einbauen.

Alternativ kann man den JavaScript-Code so schreiben, dass er erst ausgeführt wird, wenn die ganze Seite geladen wurde:

```javascript
// Führe die Funktion init aus, wenn die Seite geladen wurde
document.addEventListener('DOMContentLoaded', init, false);

function init() {
  // Hier können wir sicher sein, dass der Button schon erstellt wurde
  document.querySelector('button#submit').addEventHandler('click', () => {
    console.log('Button wurde geklickt');
  });
}
```
