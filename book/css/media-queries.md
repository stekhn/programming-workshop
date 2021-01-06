# Media Queries

Media Queries können dazu verwendet werden, um das Design einer Seite abhängig von der Darstellungsgröße zu beeinflussen. Das spielt vor allem für das responsive Webdesign eine große Rolle, da man zum Beispiel in der Smartphone-Darstellung einer Webseite weniger Informationen anzeigen möchte als in der Desktop-Darstellung einer Seite.

In diesem Beispiel wird die Seitenleiste `#sidebar` ausgeblendet sobald der Seite weniger als 600 Pixel in der Breite zur Verfügung stehen:

```css
@media (max-width: 600px) {
  #sidebar {
    display: none;
  }
}
```

📖 **Wikipedia**: [Responsive Webdesign](https://de.wikipedia.org/wiki/Responsive_Webdesign)  
📖 **MDN**: [Media Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)
