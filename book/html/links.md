# Links

Der `<a>`-Tag bezeichnet einen Hyperlink , der auf eine andere Seite oder einen Anker innerhalb der Seite verweist, angegeben durch das `href`-Attribut.

Ein Beispiel für einen Link:

```html
<p>
  Mehr Informationen zum Thema HTML gibt es auf der
  <a href="https://developer.mozilla.org/">MDN-Webseite</a>.
</p>
```

Ein Beispiel für einen Anchor:

```html
<p>
  Mehr Informationen zum Thema Anker erfahren unter dem Abschnitt
  <a href="#anchor">Anker</a>.
</p>

<p id="anchor">
  Anker sind eine großartige Möglichkeit um Inhalte auf einer Seite
  untereinander zu verlinken.
</p>
<p></p>
```

Anker beziehen sich immer auf das `id`-Attribut eines Elements und beginnen mit einer Raute `#`.

💡 _Oft sieht man auch das Attribut `target="_blank"`. Dieses dient dazu einen Link in einem neuen Fenster oder Tab zu öffnen. Grundsätzlich wird aber von der Verwendung abgeraten, da der Benutzer selbst entscheiden soll, wo er einen Link öffnet. Ist man aber auf die Verwendung von `target="_blank"` angewiesen, sollte man aus Sicherheitsgründen auf jeden Fall zusätzlich das Attribut `rel="noopener"` setzen._

📖 **CSS-Tricks**: [When to use target=”\_blank”](https://css-tricks.com/use-target_blank/)
