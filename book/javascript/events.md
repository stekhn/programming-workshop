# Events

Events sind bestimmte Aktionen oder Ereignisse, die eine bestimmte Reaktion auslösen können, wenn sie in einer JavaScript-Webseite ausgelöst werden. Diese Ereignisse können Dinge wie Klick auf einen Button, das Laden einer Seite, das Ändern eines Formularfeldes oder das Bewegen des Mauszeigers sein.

Um ein Event in JavaScript zu verarbeiten, kann man die addEventListener()-Methode verwenden. Die Syntax dafür ist folgende:

```javascript
element.addEventListener(eventType, callbackFunction);
```

- `element` ist das HTML-Element, für das das Event verarbeitet werden soll.
- `eventType` ist der Typ des Events, z.B. "click" oder "load".
- `callbackFunction` ist die Funktion, die ausgeführt wird, wenn das Event ausgelöst wird.

Ein einfaches Beispiel für ein Click-Event auf einen Button wäre:

```html
<button id="myButton">Klick mich</button>

<script>
  const button = document.querySelector("#myButton");
  button.addEventListener("click", () => {
    alert("Button wurde geklickt!");
  });
</script>
```

In diesem Beispiel wird das Button-Element ausgewählt und dann wird mit `addEventListener` angegeben, dass bei einem Klick auf den Button eine Funktion ausgeführt werden soll. Diese Funktion zeigt ein Alert mit der Meldung "Button wurde geklickt!" an.

Es ist wichtig zu beachten, dass ein Event auf ein Element nur ausgelöst werden kann, wenn das HTML-Element bereits vollständig geladen wurde. Daher muss man dafür sorgen, dass man erst nach dem Laden der Seite mit der Verarbeitung von Events beginnt. Das kann man tun, indem man die `window.onload`-Eigenschaft verwendet oder indem man das Event direkt an das `document`-Element bindet.

Events sind ein wichtiger Bestandteil jeder JavaScript-Webseite und ermöglichen es, interaktive Webseiten zu erstellen.

📖 **MDN**: [Introduction to Events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)
