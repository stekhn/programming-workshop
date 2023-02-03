# Bibliotheken

Durch Bibliotheken können Entwickler ihre Arbeit beschleunigen, indem sie auf bereits getestete und bewährte Lösungen zurückgreifen, statt jedes Mal eigenen Code schreiben zu müssen. Die meisten Bibliotheken sind für sehr bestimmte Aufgaben oder Probleme gemacht, wie zum Beispiel das Arbeiten mit Datumsangaben, Formularen oder bestimmten Datenschnittstellen. Die meisten Bibliotheken werden kostenlos und unter einen Open-Source-Lizenz angeboten.

> 💡 _Häufig bezeichnet man Bibliotheken auch als Libraries, Packages, Dependencies oder auf Deutsch Abhängigkeiten._

Bibliotheken in JavaScript können über den Paketmanager [NPM](https://www.npmjs.com/) oder über ein CDN (Content Delivery Network) eingebunden werden. NPM bietet auch einen Überblick über die verfügbaren Bibliotheken. Um npm verwenden zu können, muss jedoch zuerst [Node.js](https://nodejs.org/) installiert werden. Node.js ermöglicht es JavaScript in der Kommandozeile auszuführen. Nach erfolgreicher Installation, können Bibliotheken über folgenden Befehle installiert werden:

```shell
npm install lodash
```

Lodash ist eine Bibliothek die bei der Arbeit mit Array und Daten allgemein hilft. Nach erfolgreicher Installation kann die Bibliothek mit folgendem JavaScript-Code in den Code eingebunden werden.

In diesem Beispiel wird die Funktion `shuffle` aus der Bibliothek `lodash` importiert:

```javascript
var shuffle = require("lodash/shuffle");
```

Oder in modernem JavaScript:

```javascript
import { shuffle } from "lodash";
```

Jetzt kann die importierte Funktion `shuffle` verwendet werden, um Array zufällig zu sortieren.

```javascript
shuffle([1, 2, 3, 4]);
// => [4, 1, 3, 2]
```

Es ist auch möglich, Bibliotheken aus einem CDN (Content Delivery Network) einzubinden, ohne sie lokal zu installieren. Die Bibliothek kann über einen Script-Tag in einer HTML-Datei, meistens der `index.html`, eingebunden werden. Die Datei wird dann extern von den Server eines CDN-Anbieters wie [CDNJS](ttps://cdnjs.com/) geladen.

Beispiel:

```html
<script src="https://cdn.jsdelivr.net/npm/lodash@4.17.20/lodash.min.js"></script>
```

Nun sollte die Bibliothek über eine globale Variable verwendet werden können. Im Fall von lodash ist das ein Unterstrich, der namensgebend für die Bibliothek ist:

```javascript
_.shuffle([1, 2, 3, 4]);
// => [4, 1, 3, 2]
```

Allerdings sollte man beachten, dass externe Bibliotheken immer eine Internetverbindung benötigen. Außerdem kann das externe Einbinden von Abhängigkeiten datenschutzrechtliche Implikationen haben. Daher wird in der Regel empfohlen, Bibliotheken lokal zu installieren und über npm zu verwalten, wenn man eine stabile und performante Anwendung erstellen möchte.
