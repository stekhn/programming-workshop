# Abschnitte und Blöcke

Semantische Abschnitte helfen dabei eine Seite logisch zu strukturieren und Suchmaschinen und Screen-Readern Hinweise darauf zugeben, wie wichtig einzelne Abschnitte sind und welche Funktion sie erfüllen.

- `<header>`: Mit dem `<header>`-Element wir der Kopfbereich eines Sinnabschnitts ausgezeichnet. Er wird auch für den Kopfbereich der gesamten Website verwendet und enthält üblicherweise das Seitenlogo, einen Slogan und ein `<nav>`-Menü.
- `<nav>`: Das `<nav>`-Element kennzeichnet die Seitennavigation. Meistens ist dies eine Liste interner Links.
- `<article>`: Abgeleitet von dem Artikel für die Zeitung werden alle in sich abgeschlossenen Inhalte, wie zum Beispiel Beiträge in einem Blog mit dem `<article>`-Element umfasst.
- `<section>`: Beschreibt einen thematischen Abschnitt eines Dokuments. Jede `<section>` sollte daher auch eine Überschrift haben.
- `<aside>`: Inhalte, die nicht zum Hauptinhalt einer Seite zählen, werden mit dem  `<aside>`-Element ausgezeichnet. Mit `<aside>` kann beispielsweise eine Sidebar auf der Website eingerichtet werden.
- `<footer>`: Die Informationen im Fußbereich der Website oder eines Sinnabschnitts werden mit dem `<footer>`-Element umschlossen.
- `<main>`: Definiert den Hauptinhalt der Seite. Es ist nur ein `<main>` Element pro Seite zulässig.

Ein Beispiel:

```html
<!DOCTYPE html>
<html lang="de">
<head>
 <title>Titel der Webseite</title>
</head>
<body>
  <header>
    <h1>Überschrift für die gesamte Webseite</h1>
    <nav>
      <ul>
        <li><a href="#">Link</a></li>
        <li><a href="#">Link</a></li>
        <li><a href="#">Link</a></li>
      </ul>
    </nav>
  </header>
  <article>
    <h2>Überschrift des ersten Artikels</h2>
      <p>Text des ersten Artikels</p>
  </article>
  <article>
    <h2>Überschrift des zweiten Artikels</h2>
    <p>Text des zweiten Artikels</p>
  </article>
  <aside>
    <h3>Überschrift Sidebar</h3>
    <p>Text in der Sidebar</p>
  </aside>
  <footer>
    <h3>Überschrift Footer</h3>
    <p>Text im Footer</p>
  </footer>
</body>
</html>
```

Sehr häufig sieht man auch das unspezifische Blockelement `<div>`. Dieses wird für Abschnitte verwendet, welche keine inhaltliche Bedeutung haben. Oftmals dient es vor allem dazu Container zu erstellen, die dann über CSS gestylt werden können.

💡 *Semantisches HTML ist die Grundlage einer barrierefreien Webseite. Gerade Menschen mit Sehbehinderungen nutzen oftmals technisches Hilfsmittel wie Screen-Reader, welche auf semantische Auszeichnungen, aber auch sinnvolle Bildbeschreibungen, angewiesen sind.*

📖 **MDN**: [HTML Dokumentation](https://developer.mozilla.org/en-US/docs/Web/HTML/HTML5/HTML5_element_list#Abschnitte_(Sections))  
📖 **Kulturbanause**: [HTML-Elemente und Semantik](https://blog.kulturbanause.de/2008/01/html-elemente-und-semantik/)
