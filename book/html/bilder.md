# Bilder

Bilder sind auf einer Webseite mindestens ebenso wichtig wie Texte. In HTML werden Bilder mit dem `<img>`-Element eingebunden. Dieses benötigt im Gegensatz zu den meisten anderen Elementen keinen schließenden Tag und sollte immer ein ein `src`- und ein `alt`-Attribut besitzen.

Ein Beispiel:

```html
<img src="image.jpg" alt="Beispielbild" />
```

Das `alt`-Attribut ist der Alternativtext eines Bildes. Suchmaschinen benutzen dieses Attribut, um den Bildinhalt zu erkennen, da die Bilddateien selbst in der Regel nicht direkt ausgelesen werden können. Für sehbehinderte Nutzer trägt das `alt`-Attribut zur Barrierefreiheit bei. Dadurch lassen sich Webseiten mit einem Screenreader vorlesen.

Bilder lassen sich mit dem `src`-Attribut aus verschiedenden Quellen laden. Im Beispiel oben wird das Bild aus dem Hauptverzeichnis der Webseite geladen, wo sich auch die `index.html`-Datei befindet. Oftmals werden Bilder jedoch in einem Unterordner `images` (oder so ähnlich) gespeichert. In diesem Fall muss das `src`-Attribut entsprechend angepasst werden.

```html
<img src="images/image.jpg" alt="Beispielbild" />
```

Bilder können jedoch auch direkt von anderen Webseiten geladen werden:

```html
<img
  src="https://de.wikipedia.org/static/images/project-logos/dewiki.png"
  alt="Wikipedia-Logo"
/>
```

Die Größe und Position eine Bildes lassen sich über CSS-Regeln definieren. Für Bilder ist das Thema Responsivität sehr wichtig. Dabei geht es darum, dass sich ein Bild an die verschiedenen Bildschirmgrößen (Smartphone, Tablet, Desktop-Computer) anpasst.

> 💡 _Die Dateigröße von Bildern trägt maßgeblich zur Gesamtgröße und damit auch Ladezeit einer Webseite bei. Daher empfiehlt es sich die Bilder vorher auf die maximal notwendige Auflösung zu verkleinern und im JPEG-Format (85 bis 95 % Kompression) abzuspeichern._

📖 **MDN**: [Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)  
📖 **MDN**: [Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)
