# iFrames

iFrames können dazu verwendet werden um Inhalte von einer anderen Webseite einzubetten.

Beispiel für eine eingebettete Karte (OpenStreetMap):

```html
<iframe
  width="640"
  height="360"
  src="https://www.openstreetmap.org/export/embed.html?bbox=11.4071%2C48.0284%2C11.7191%2C48.2326&layer=mapnik"
></iframe>
```

Beispiel für ein YouTube-Embed:

```html
<iframe
  width="640"
  height="360"
  src="https://www.youtube.com/embed/jpmeWXISU5E?&rel=0&showinfo=0"
  frameborder="0"
  allowfullscreen
></iframe>
```

> 💡 _Meistens empfiehlt es sich die Breiten- und Höhenangaben in einem iFrame wegzulassen und die Größe über eine CSS-Regel zu definieren. Das ist deutlich flexibler und erlaubt auch prozentuale Größenangeben wie `width: 100%;`_

Mittlerweile verwenden viele Seiten andere Methoden um ihre Inhalte zum Einbetten anzubieten. Hier ein Beispiel für das Einbetten eines Posts von Twitter:

```html
<blockquote class="twitter-tweet" data-lang="de">
  <p lang="en" dir="ltr">
    &quot;Weeks of coding can save you hours of planning.&quot; - Unknown
  </p>
  &mdash; Programming Wisdom (@CodeWisdom)
  <a
    href="https://twitter.com/CodeWisdom/status/1031158088018083841?ref_src=twsrc%5Etfw"
    >19. August 2018</a
  >
</blockquote>
<script
  async
  src="https://platform.twitter.com/widgets.js"
  charset="utf-8"
></script>
```

📖 **MDN**: [iFrame Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe)  
📖 **MDN**: [Multimedia and Embedding](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding)
