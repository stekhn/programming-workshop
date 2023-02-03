# Shorthand-Eigenschaften

Vor allem wenn man mit Größenangaben arbeiten, erleichtern einem sogenannte _Shorthand-Properties_ die Arbeit ungemein. Grundsätzlich kann man die Außenabstände eine Containers einfach einzeln angeben:

```css
.info-box {
  margin-top: 20px;
  margin-right: 20px;
  margin-bottom: 20px;
  margin-left: 20px;
}
```

Wenn diese Werte aber gleich sind, kann man aber auch folgende Abkürzung verwenden, um die Werte für alle Seiten auf einmal zu setzen:

```css
.info-box {
  margin: 20px;
}
```

Wenn jedoch der untere und obere Abstand größer sein soll, kann man dies mit folgender Abkürzung erreichen:

```css
.info-box {
  margin: 40px 20px;
}
```

Wenn der unter Abstand noch größer sein soll, kann man diese mit der dreifachen Shorthand-Property festlegen:

```css
.info-box {
  margin: 40px 20px 60px;
}
```

Man kann auch alle Abstände mit nur einer Eigenschaft setzten:

```css
.info-box {
  margin: 40px 20px 60px 10px;
}
```

Für die Eigenschaften `margin` und `padding` gibt es also vier verschieden Shorthand-Properties:

- `margin: (top, right, bottom, left);`
- `margin: (top, bottom) (right, left);`
- `margin: top (right, left) bottom;`
- `margin: top right left bottom;`

> 💡 _Es gibt noch viele weitere CSS-Eigenschaften (`background`, `font`, `box-shadow`), welche bestimmte Shorthand-Properties unterstützen. Gerade am Anfang aber sollte man eher sparsam damit umgehen._

📖 **MDN** [Shorthand Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Shorthand_properties)
