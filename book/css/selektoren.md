# Selektoren

Selektoren dienen dazu bestimmte Elemente oder Gruppen von Elementen auszuwählen, um sie zu stylen. Ein wichtiges Konzept dabei ist Spezifität. Spezifität bedeutet, dass wenn es mehrere Style-Regeln für ein Element gibt, wird die jeweils spezifiste Regel angewandt. Universalselektor sind am unspezifisten, ID-Selektoren und Inline-Styles am spezifisten und daher am stärkesten. Hier die Selektoren in aufsteigender Spezifität:

- **Universalselektor**: `*`
- **Typselektoren**: `element`
- **Klassenselektoren**: `.class`
- **Attributselektoren**: [attribute] oder [attribute="value"]
- **Pseudoklassen**: `element::pseudo`
- **ID-Selektoren**: `#id`
- **Inline-Styles**: `<element style>`

Um das ganze noch ein bisschen komplizierter zu machen, kann man Selektoren auch miteinandern kombinieren:

- `A, B`: Es wird A und B selektiert.
- `A B`: Es wird B (*child*) selektiert, welches in der Hierarchie irgendwo unter A (*parent*) liegt

Eher seltener zum Einsatz kommen diese Selektorkombinationen:

- `A > B`: Es wird B (*direct child*)selektiert, welches in der Hierarche unmittelbar unter A (*parent*) liegt.
- `A ~ B`: Es wird B (*sibling*) selektiert, welches in der Hierarchie neben A (*sibling*) liegt.
- `A + B`: Es wird B (*direct sibling*) selektiert, welches in der Hierarchie direkt neben A (*sibling*) liegt.

Um die grundlegende Konzepte zu verdeutlichen, erstellen wir drei unterschiedliche Listen. Diese sollen gestylt werden.

```html
<ul id="todo-list">
  <li class="list-item">Gemüse einkaufen</li>
  <li class="list-item">Fahrrad reparieren</li>
  <li class="list-item">Zahnarzttermin vereinbaren</li>
</ul>

<ul id="name-list">
  <li class="list-item">Philipp</li>
  <li class="list-item">Oskar</li>
  <li class="list-item">Marlene</li>
</ul>

<ul>
  <li>München</li>
  <li>Hamburg</li>
  <li>Berlin</li>
</ul>
```

Schriftart für die ganze Webseite setzen:

```css
body {
  font-family: Arial, Helvetica, sans-serif;
}
```

Für alle Listen das Aufzählungszeichen und den Innenabstand ändern:

```css
ul {
  list-style-type: square;
  list-style-position: inside;
  padding: 0;
}
```

Alle Elemente mit Klasse `.list-item` bekommen einen graue Textfarbe und einen größeren Außenabstand.

```css
.list-item {
  margin: 1em 0;
  color: grey;
}
```

Die Liste mit der ID `#todo-list` bekommt einen hellblauen Hintergrund:

```css
#todo-list {
  background: aliceblue;
}
```

Die Liste mit der ID `#todo-list` bekommt einen hellblauen Hintergrund:

```css
#name-list {
  background: antiquewhite;
}
```

Die Listeneinträge der ToDo-Liste bekommen eine blaue Textfarbe. Die ursprüngliche Farbe Grau wird automatisch überschrieben. Hier könnte man auch `#todo-list li` schreiben.

```css
#todo-list .list-item {
  color: darkblue;
}
```

Einträge mit der in der ToDo-Liste mit der Klasse `done` werde grün eingefärbt. Der vorher gesetze Farbwert blau wird nochmals überschrieben. Auch hier könnte man auch `#todo-list li.done` schreiben.

```css
#todo-list .list-item.done {
  color: darkgreen;
}
```

💡 *Man kann einzelne CSS-Regeln auch mit dem Attribut `!important` erzwingen `.error { color: red !important; }`. Das ist aber in den wenigsten Fällen empfehlenswert. Ist man häufiger darauf angewiesen `!important` zu verwenden, deutet dass auf schlecht strukturiertes HTML oder CSS hin.*

📖 **MDN** [Combinators and selector lists
](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Combinators_and_multiple_selectors)
