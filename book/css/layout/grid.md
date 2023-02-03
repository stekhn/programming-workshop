# Grid

CSS Grid ist ein weiteres Layout-Modell in CSS, das es Entwicklern ermöglicht, komplexe Layouts mithilfe eines Gestaltungsrasters zu erstellen, in dem Elemente in Zeilen und Spalten positioniert werden können.

Um CSS Grid zu verwenden, wird einem Container-Element die CSS-Eigenschaft "display: grid" zugewiesen. Dann kann man die Größe der Zeilen und Spalten des Rasters definieren, indem man die CSS-Eigenschaften "grid-template-columns" und "grid-template-rows" verwendet. Die Elemente innerhalb des Containers können dann positioniert werden, indem man die Eigenschaften "grid-column" und "grid-row" zuweist.

Zum Beispiel:

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: auto auto;
}

.item1 {
  grid-column: 1 / 2;
  grid-row: 1 / 2;
}

.item2 {
  grid-column: 2 / 3;
  grid-row: 1 / 3;
}
```

In diesem Beispiel wird ein 3-spaltiges Raster mit zwei Zeilen erstellt. Das erste Element (`.item1`) wird in der linken oberen Hälfte und das zweite Element (`.item1`) wird in rechten oberen und unteren Hälfte des Rasters platziert.

```text
+------------+------------+
| .item1     | .item2     |
+------------+            |
|            |            |
+------------+------------+
```

CSS Grid bietet auch fortgeschrittene Funktionen wie gleichmäßige oder ungleichmäßige Spaltenverteilung und automatisches Rasterlayouts. Es ist ein mächtiges Werkzeug für responsive Layouts und komplexe Designs.

📖 **MDN**: [Grids](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grids)  
📖 **CSS-Tricks**: [A Complete Guide to CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
