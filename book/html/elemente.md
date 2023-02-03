# Elemente

HTML unterstützt zur Zeit etwa 130 verschiedene Elemente. In der Praxis braucht man aber meistens nur einen kleinen Teil davon. Im Folgenden werden nur eine Handvoll Elemente vorgestellt, die man als Einsteiger braucht um ein einfache Webseite zu bauen.

Grundsätzlich besteht ein Element aus dem Element-Tag und bei bestimmten Elementen zusätzlich noch aus verschiedenen Attributen und Werten. Hier ein Beispiel für ein Bild-Tag `<img>` mit zwei Attributen `src` und `alt`:

```html
<img src="image.jpg" alt="Beispielbild" />
```

`src` ist das sogenannte Attribut und `image.jpg` der Wert. Zusammen geben sie an wo sich das Bild befindet, welches eingebunden werden soll. Das Attribut `alt` ist die Bildbeschreibung, welche für die Barrierefreiheit wichtig ist und auch dann angezeigt wird, wenn das Bild nicht geladen werden kann.

`<img>` gehört zu den Elementen, welche keinen schließenden Tag benötigen. Davon gibt es aber sehr wenige. Die wichtigsten sind: `<img>`, `<input>`, `<br>`, `<hr>`, `<meta>` und `<link>`.

Die meisten Elemente benötigen einen schließenden Tag. Ein Beispiel dafür ist das `<a>`-Element, welches für Links (Anchor) verwendet wird. Hier verwenden wir das `<a>`-Element innerhalb eines `<p>`-Paragraphen. Das Verschachteln von unterschiedlichen Elementen ist typisch für HTML:

```html
<p>
  Mehr Informationen zum Thema HTML gibt es auf der
  <a href="https://developer.mozilla.org/">MDN-Webseite</a>.
</p>
```

Der `<a>`-Tag umschließt den Linktext _MDN-Webseite_. Das Attribut `href` gibt an, wohin der Link führen soll. Weiter unten gibt es mehr Informationen zur Verwendung von Links. Welche Elemente es gibt und welche Attribute diese besitzen, lässt sich auf den Seiten des Mozilla Developer Networks nachschlagen: 📖 [HTML Element Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

> ⚠️ _Fehlende schließende Tags sind gerade für Einsteiger eine häufige Fehlerquelle und können das Layout einer Seite zerschießen. Das Problem wird dadurch verstärkt, dass der Browser selbstständig versucht ungültiges HTML zu reparieren und offene Tags wieder zu schließen. Im Zweifelsfalls hilft es, das eigene HTML auf nicht geschlossenen Tags hin zu überprüfen. Ein gute Code-Editor kann dabei helfen, solche Fehler frühzeitig zu erkennen._
