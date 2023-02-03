# Flexbox

CSS Flexbox ist ein Layout-Modell in CSS, das es Entwicklern ermöglicht, flexible Layouts zu entwickeln. Es ermöglicht das Ausrichten, Anordnen und Skalieren von Elementen innerhalb eines Containers.

Um Flexbox zu verwenden, wird einem Container-Element die CSS-Eigenschaft "display: flex" zugewiesen. Von hier aus kann man weitere Eigenschaften wie "justify-content" (Ausrichtung entlang der Hauptachse), "align-items" (Ausrichtung entlang der Querachse) und "flex-wrap" (Zeilenumbruch bei Bedarf) verwenden, um die Kinder-Elemente innerhalb des Containers anzupassen.

Ein Beispiel:

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
```

Diese Einstellungen zentrieren alle Elemente eines Containers sowohl horizontal (`justify-content: center`) als auch vertikal (`align-items: center`). Sind zu viele Element in einem Container, dürfen die Elemente in die nächste Zeile umbrechen (`flex-wrap: wrap`).

Flexbox ist gute Alternative zu CSS Floats und erleichtert das Ausrichten von Elementen im Seitenlayout enorm.

📖 **MDN**: [Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)  
📖 **CSS-Tricks**: [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
