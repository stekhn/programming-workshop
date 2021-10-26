# Meta-Tags

Meta-Tags sind die Grundlage für eine gute Suchmaschinen-Optimierung (SEO). Sie helfen den Suchmaschinen dabei zu verstehen, was der Kerninhalt einer Webseite ist. Außerdem ermöglichen sie, dass in sozialen Netzwerken wie Twitter oder Facebook eine Vorschau des Webseiteninhalts, meistens mit Bild, angezeigt werden können ([Beispiel](https://twitter.com/derspiegel/status/1453093827212832773)).

Die Meta-Tags werden im `<head>`-Bereich einer Webseite eingebunden:

```html
  <meta name="author" content="Steffen Kühne" />
  <meta name="title" content="Informationen zur Schwarzfußkatze" />
  <meta name="description" content="Die Schwarzfußkatze ist die kleinste afrikanische Katze. Hier erfahren Sie alles über ihr Aussehen, ihren Lebensraum und warum sie bedroht ist." />
  <meta name="keywords" content="Schwarzfußkatze, kleinste Katze, Afrika, Aussehen, Lebensraum, Verbreitung, bedroht, Schwarze Liste" />

  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:site" content="@stekhn" />
  <meta name="twitter:creator" content="@stekhn" />
  <meta name="twitter:title" content="Informationen zur Schwarzfußkatze" />
  <meta name="twitter:description" content="Die Schwarzfußkatze ist die kleinste afrikanische Katze. Hier erfahren Sie alles über ihr Aussehen, ihren Lebensraum und warum sie bedroht ist." />
  <meta name="twitter:url" content="https://schwarzfusskatze.info/" />
  <meta name="twitter:image" content="https://schwarzfusskatze.info/vorschau.jpg" />

  <meta property="og:type" content="article" />
  <meta property="og:locale" content="de_DE" />
  <meta property="og:site_name" content="BR" />
  <meta property="og:title" content="Informationen zur Schwarzfußkatze" />
  <meta property="og:description" content="Die Schwarzfußkatze ist die kleinste afrikanische Katze. Hier erfahren Sie alles über ihr Aussehen, ihren Lebensraum und warum sie bedroht ist." />
  <meta property="og:url" content="https://schwarzfusskatze.info/" />
  <meta property=" og:image" content="https://schwarzfusskatze.info/vorschau.jpg" />
```

📖 **metatags.io**: [Metatags erstellen](https://metatags.io/)  
📖 **CSS-Tricls**: [The Essential Meta Tags for Social Media](https://css-tricks.com/essential-meta-tags-social-media/)