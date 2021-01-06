# Position

Die CSS-Eigenschaft `position` gibt die Art der Positionierungsmethode an, die für ein Element verwendet wird. Dabei kann ein Element, ähnlich wie bei `float`, aus dem normalen Textfluss herausgenommen werden. Folgenden Eigenschaften stehen zur Verfügung:

- `static`: Standardwert. Das Element ist im normalen Fluss. Die Eigenschaften top, right, bottom oder left haben keine Auswirkungen.
- `relative`: Das Element wird vom normalen Fluss aus verschoben und hat keinen Einfluss auf andere Elemente, da an der ursprünglichen Position Platz gelassen wird. Bei table-*-group, table-row, table-column, table-cell, und table-caption Elementen ist kein Effekt definiert.
- `absolute`: Das Element wird aus dem normalen Fluss gelöst und unabhängig verschoben. Dabei können andere Elemente verdeckt werden. Diese verhalten sich so, als ob das Element nicht vorhanden wäre und lassen keinen Platz für das Element.
- `fixed`: Die Verschiebung orientiert sich am Viewport. Das Element wird aus dem normalen Fluss gelöst und bleibt auch beim Scrollen an seiner fest definierten Position. Beim Drucken wird das Element auf jeder Seite an der positionierten Stelle angezeigt.
- `sticky`: Eine Mischung zwischen fixed und relative: Das Element wird vom normalen Fluss aus verschoben und hat keinen Einfluss auf andere Elemente, solange es sich innerhalb des Viewports befindet. Sobald es sich ausserhalb befindet, wird das Element aus dem normalen Fluss gelöst und bleibt so beim Scrollen an seiner fest definierten Position.

Wird ein Elemente mit `absolute`, `fixed` oder `sticky` aus dem normalen Textfluss genommen, muss mit den Eigenschaftten `top`, `right`, `bottom` oder `left` angegeben werden, wo es auf der Seite erscheinen sollen.

Hier ein Beispiel für ein fixierte Navigationsleiste mit drei Menüpunkten die immer oben im Browserfenster angezeigt wird, auch wenn den Benutzer nach unten scrollt:

```html
<nav id="navbar">
  <a href="#home">Home</a>
  <a href="#news">News</a>
  <a href="#contact">Contact</a>
</nav>
```

```css
.navbar {
  position: fixed;
  top: 0;
  width: 100%;
  background: black;
}

.navbar a {
  float: left;
  display: block;
  color: white;
  text-align: center;
  padding: 1em;
  text-decoration: none;
}
```

📖 **MDN**: [Position](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)  
📖 **MDN**: [Top, Right, Left, Bottom](https://developer.mozilla.org/en-US/docs/Web/CSS/top)
