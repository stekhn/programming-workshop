# Einbinden

CSS kann auf deiner eigene Seite auf zwei Wegen eingebunden werden. Für kleine Webprojekte kann man CSS-Regel direkt in einem `<style>`-Element, meistens im `<head>`-Bereich einer Seite, definieren:

```html
<!DOCTYPE html>
<html lang="de">
  <head>
    <title>Titel der Webseite</title>

    <style>
      body {
        font-family: Arial, Helvetica, sans-serif;
      }

      h1 {
        color: red;
      }
    </style>
  </head>
  <body>
    <h1>Überschrift</h1>
  </body>
</html>
```

Für größere Projekte empfiehlt es sich jedoch die CSS-Regel in einer eigenen CSS-Datei zu schreiben und diese über einen `link`-Tag einzubinden:

```html
<!DOCTYPE html>
<html lang="de">
  <head>
    <title>Titel der Webseite</title>
    <link href="style.css" rel="stylesheet" />
  </head>
  <body>
    <h1>Überschrift</h1>
  </body>
</html>
```

💡 _Man kann `<style>` und `<link>`-Tags auch an anderer Stelle im HTML verwenden. Durch das Einbauen im `<head>`-Bereich wird jedoch sichergestellt, dass die Styles geladen sind, bevor die Seite dargestellt wird. Das ist oftmals wichtig, wenn man auf darauf angewiesen ist, dass ein Element eine bestimmte Höhe hat, bevor man damit arbeitet._
