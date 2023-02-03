# DOM-Manipulation

DOM-Manipulation bezeichnet das Ändern von Webseiten-Elemente mithilfe von JavaScript. Der DOM (Document Object Model) ist, vereinfacht gesagt, die Struktur einer Webseite, wenn man sie als Baum mit Elementen und Unterelementen darstellen würden. Der Browser stellt bestimmte Methoden bereit, um auf den DOM zuzugreifen und Elemente verändern zu können. Neue Elemente können hinzugefügt, bestehende Elemente können geändert oder entfernt werden.

Zum Auswählen einzelner oder mehrere Elemente gibt es folgende Möglichkeiten:

1. **getElementById:** Diese Methode sucht nach einem Element auf der Basis seiner ID. Sie gibt das erste gefundene Element mit dieser ID zurück. Beispiel: `document.getElementById("meineId")`
2. **getElementsByTagName:** Diese Methode sucht nach allen Elementen mit einem bestimmten HTML-Tag. Sie gibt ein HTMLCollection (ähnlich einem Array) mit allen gefundenen Elementen zurück. Beispiel: `document.getElementsByTagName("p")`
3. **querySelector:** Diese Methode ist eine erweiterte Version von getElementById und getElementsByTagName. Man kann mittels eines CSS-ähnlichen Selektors nach einem Element suchen. Sie gibt das erste gefundene Element zurück. Beispiel: `document.querySelector("#meineId .meineKlasse")`
4. **querySelectorAll:** Diese Methode ist eine erweiterte Version von getElementsByTagName. Man kann mittels eines CSS-ähnlichen Selektors nach allen passenden Elementen suchen. Sie gibt ein NodeList (ähnlich einem Array) mit allen gefundenen Elementen zurück. Beispiel: `document.querySelectorAll(".meineKlasse")`

> 💡 _`querySelector` und `querySelectorAll` sind die flexibelsten Methoden, um Elemente auszuwählen. Gerade für den Anfang lohnt es sich, einfach mit diesen beiden Methoden zu arbeiten und zu lernen, wie man Selektoren dafür schreibt. Die Selektoren funktionieren im Prinzip genauso, wie man sie in CSS schreiben würde._

Um ein Element mit JavaScript hinzuzufügen, muss zunächst ein neues Element erstellt werden. Dies kann mit der Methode `document.createElement(elementName)` erreicht werden, wobei `elementName` der gewünschte Name des Elements ist, zum Beispiel "h1" für eine Überschrift. Für das neu erstellte Element können dann bestimmte Eigenschaften festgelegt werden, wie Inhalt, ID, Klasse oder andere Attribute.

Zum Hinzufügen des Elements zur Seite kann es an ein bestehendes Element angehängt werden, indem die Methode `appendChild` des Elternelements, in diesem Fall der `body`, aufgerufen wird und das neue Element als Argument übergeben wird.

Beispiel:

```javascript
var newHeadline = document.createElement("h1");
newDiv.textContent = "Ich bin ein neue Überschrift";
newDiv.id = "headline";
document.body.appendChild(newHeadline);
```

Um eine bereits bestehende Überschrift mit JavaScript zu ändern, kann man das entsprechende Element über seine ID oder Klasse mittels `document.getElementById` oder `document.getElementsByClassName` auswählen. In diesen Beispielen wird eine Überschrift mittels ihrer ID ausgewählt und entsprechend verändert. Auf ähnliche Weise kann man auch Überschriften, die mittels Klasse ausgewählt wurden, verändern.

Ändern des Textes:

```javascript
const headline = document.querySelector("#headline");
headline.innerHTML = "Neuer Überschriftentext";
```

Ändern der Klasse:

```javascript
const headline = document.querySelector("#headline");
headline.className = "new-class";
Ändern der Hintergrundfarbe:
```

Ändern der Hintergrundfarbe:

```javascript
const headline = document.querySelector("#headline");
headline.style.backgroundColor = "lightblue";
```

Um die oben angelegte Überschrift zu löschen, muss man dessen Eltern-Element verwenden und dessen `removeChild`-Methode aufrufen. Hier ist ein Beispiel:

```javascript
const headline = document.querySelector("#headline");
var parent = headline.parentNode;
parent.removeChild(headline);
```

Dass jeweils das Eltern-Element ermittelt werden muss, um ein Element zu löschen ist leider ein wenig aufwendig.

📖 **MDN**: [Manipulating documents](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Manipulating_documents)
