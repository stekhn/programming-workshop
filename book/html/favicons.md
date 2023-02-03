# Favicons

Als Favicon wird das kleine Symbol neben dem Titel in der Kopfzeile eines Browsers oder eines Browser-Tab bezeichnet. Favicons sind ein wichtiges Branding-Element und helfen Benutzern dabei eine Webseite schnell wiederzufinden.

Leider gibt es nicht den einen Standard, wie man Favicons auf einer Seite einbinden. Verschiedene Geräte- und Browserhersteller verwenden verschieden Größenverhältnisse und Bildformate.

Hier ein einfaches Beispiel für Favicons, welche in den meisten modernen Browsern funktionieren sollte. Die Meta-Tags werden im `<head>`-Bereich einer Webseite eingebunden:

```html
<link rel="icon" href="/favicon.ico" sizes="any" />
<link rel="icon" href="/favicon.svg" type="image/svg+xml" />
<link rel="apple-touch-icon" href="/apple-touch-icon.png" />
```

📖 **Favicon Generator**: [Create Favicons for different devices](https://realfavicongenerator.net/)  
📖 **CSS-Tricks**: [How to Favicon in 2021](https://css-tricks.com/how-to-favicon-in-2021/)
