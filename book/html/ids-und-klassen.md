### IDs und Klassen
Es gibt zwei spezielle Attribute die auf jedes Element angewendet werden können: `id` und `class`. IDs und Klassen sind essenzielle Konzepte um Elemente eindeutig identifiziert zu machen. Dies ist vor allem in Verbindung mit CSS und JavaScript relevant, wo man einen bestimmten Style oder eine bestimmte Funktionalität nur auf bestimmte Argumente anwenden möchte. IDs dürfen jeweils nur einmal vergebene werden, Klassen mehrfach. Hier ein Button mit einer ID, der genau eine Aktion auslöst:

```html
<button id="submit">Abschicken</button>
```

Im Gegensatz dazu werden Klassen für Elemente verwendet, welche den gleichen Style oder die gleiche Funktion haben sollen:

```html
<ul>
  <li class="list-item">Gemüse einkaufen</li>
  <li class="list-item">Fahrrad reparieren</li>
  <li class="list-item">Zahnarzttermin vereinbaren</li>
</ul>
```

Ein Element kann auch mehrere Klassen haben. In diesem Fall dient beispielsweise die Klasse `list-item` nur dazu das Element zu stylen. Die Klasse `removable` kann hingegen einen funktionelle Aspekt haben, um beispielsweise zu ermöglichen, dass der Listeneintrag gelöscht werden kann:

```html
<ul>
  <li class="list-item removable">Gemüse einkaufen</li>
  <li class="list-item removable">Fahrrad reparieren</li>
  <li class="list-item removable">Zahnarzttermin vereinbaren</li>
</ul>
```

In CSS und JavaScript wählt man IDs jeweils mit einer Raute aus `#id` und Klassen mit einem Punk `.class`.

CSS-Beispiel:

```css
#submit {
  background: red;
}

.list-item {
  color: green;
}
```

JavaScript-Beispiel:

```javascript
// Einen Button nach ID auswählen
document.querySelector('#submit')

// Alle Listeneinträge nach Klasse auswählen
document.querySelectorAll('.removable')
```
