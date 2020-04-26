### Text
Gerade für Journalisten sind dies die wohl wichtigten HTML-Elemente. Grundsätzlich besteht 

- `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`: Überschriften in absteigender Hierarchie und Textgröße. Eine Hauptüberschrift ist meistens `<h1>` oder `h2`, während man für Zwischentitel eher eine `h3` verwenden würden.
- `<p>`: Ein Textabschnitt und damit wohl das am häufigsten verwenden HTML-Element.

Um innerhalb des Texts bestimmte Abschnitte oder Wörter hervorzuheben, gibt es folgenden Auszeichnungselemente:

- `<strong>` Markiert besonders wichtigen (stark hervorgehobenen) Text und wird meistens fettgedruckt dargestellt.
- `<em>` Steht für hervorgehobenen Text (*emphasis*) und wird standardmäßig kursiv dargestellt.

Ein Beispiel:

```html
<h1>Überschrift</h1>
<p>Paragraph mit normalem Fließtext und einer <strong>Hervorhebung<strong></p>
```

💡 *Meistens sind drei Überschriftengrößen (`<h1>`, `<h2>`, `<h3>`) völlig ausreichend.*

💡 *Von der Verwendung der alten Texthervorhebungen `<i>` (kursiv), `<b>` (fett) und `<u>` (unterstrichen) wird abgeraten, da sie keine semantische Bedeutung haben und nur das Aussehen eine Textabschnitts beeinflussen.*
