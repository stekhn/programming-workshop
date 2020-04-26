### Formulare
Formulare und die dazugehörigen Elemente sind Grundlage um Benutzereingaben zu verarbeiten. Formulare sind nicht nur im Bereich E-Commerce wichtig sondern auch um interaktive Webprojekte zu realisieren. Hier eine Auswahl der wichtigsten Eingabeelemente:

- `<form>`: Markiert ein Formular. Formulare bestehen typischerweise aus einer Reihe von Kontrollelementen, deren Werte zur weiteren Verarbeitung an einen Server übertragen werden.
- `<label>`: Kennzeichnet die Beschriftung für ein Formular-Kontrollelement (z.B. Texteingabefelder).
- `<input>`: Steht für ein Feld für Benutzereingaben eines bestimmten Typs. Der Typ (Radiobutton, Ankreuzfeld, Texteingabe, etc.) wird anhand des type-Attributs angegeben.
- `<button>`: Markiert einenButton .
- `<select>`: Kennzeichnet ein Kontrollelement, mit dem aus einer Reihe von Optionen ausgewählt werden kann.
- `<datalist>`: Steht für eine Sammlung vordefinierter Optionen für andere Kontrollelemente.
- `<option>`: Steht für eine Auswahloption innerhalb eines `<select>`-Elements, oder einen Vorschlag innerhalb eines `<datalist>`-Elements.
- `<progress>`: Ein Element zur Fortschrittsanzeige einer bestimmten Aufgabe.

Ein einfaches Beispiel für Kommentarfeld:

```html
<form id="comment" name="comment" action="/save-comment" method="post">
  <div>
    <label for="name">Name:</label>
    <input type="text" id="name" name="user_name">
  </div>
  <div>
    <label for="mail">E-mail:</label>
    <input type="email" id="mail" name="user_mail">
  </div>
  <div>
    <label for="msg">Nachricht:</label>
    <textarea id="msg" name="user_message"></textarea>
  </div>
  <div class="button">
    <button type="submit">Kommentar speichern</button>
  </div>
</form>
```

In diesem Beispiel gehen wir davon aus, dass der Server einen Endpunkt `/save-comment` bereitstellt, der die Benutzereingaben entgegennimmt und speichert. Das ist aber nicht immer der Fall. Alternativ kann auch eine JavaScript-Funktion verwendet werden, um die Benutzereingeben zu verarbeiten.

Dazu müssen die `action`- und `method`-Attribute des Formulars im HTML entfernt werden:

```html
<form id="comment">
```

Um eine Aktion auszulösen, wenn der Submit-Button geklickt wird, muss ein Event-Handler registriert werden: 

```html
<script>
  document.querySelector('#comment').addEventListener('submit', handleSubmit)

  function handleSubmit(e) {
    var form = e.target;

    // Formulardaten auslesen
    var userName = form.querySelector('[name="user_name"]').value;
    var userMail = form.querySelector('[name="user_mail"]').value;
    var userComment = form.querySelector('[name="user_comment"]').value;

    // Formulardaten ausgeben
    console.log(userName, userMail, userComment);

    // Verhindern, dass die Seite neu geladen wird
    e.preventDefault();
    return false;
  }
</script>
```

💡 *Sobald es um das Verabeiten von Benutzereingaben geht, kommt man fast nicht mehr darum herum JavaScript zu verwenden. Gute Formulare zu bauen ist sehr aufwendig, vor allem wenn es um darum geht das – standardmäßig sehr hässliche – Design der Eingabeelemente anzupassen. Hier empfiehlt es sich eine Front-End-Bibliothek wie [Bootstrap](https://getbootstrap.com/), [Foundation](https://foundation.zurb.com/), [Bulma](https://bulma.io/) oder [UIKit](https://getuikit.com/) einzusetzen.*

📖 **MDN**: [Form Guide](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms)   
📖 **FreeCodeCamp**: [A step-by-step guide to getting started with HTML forms](https://medium.freecodecamp.org/a-step-by-step-guide-to-getting-started-with-html-forms-7f77ae4522b5)   
📖 **Tuts+**: [Best Form Practices for Beginners](https://code.tutsplus.com/tutorials/20-html-forms-best-practices-for-beginners--net-6593)
