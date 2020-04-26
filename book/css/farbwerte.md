### Farbwerte

Genauso wie Größenangaben lassen sich Farbwerte über verschiedenen Einheiten definieren. Hier ist es vor allem nützlich, wenn sich mit der sehr gängigen [hexadezimalen Farbdefinition](https://de.wikipedia.org/wiki/Hexadezimale_Farbdefinition) auseinandern gesetzt hat. Die Beispiele benutzen alle den gleich blauen Farbton:

- `navy`: Es gibt eine Liste an vordefinierten Farbwerten, die alle über ihren jeweiligen Namen verwendet werden können. Sehr praktisch, da einfach im Code zu lesen.
- `#000080`: Mit der hexadezimalen Farbdefinition lassen sich über 16 Millionen Farben (256^3) darstellen. Die ersten beiden Ziffern geben den Rotwert, die mittleren beiden Ziffern den Grünwert und die letzten beiden Ziffern den Blauwert an. Die Ziffernpaare geben jeweils einen Hexadezimalwert zwischen `00` (0) und `FF` (255) an. Farbwerte bei den alle Ziffernpaare gleich sind lassen sich auf drei Stellen verkürzen, wie bei diesem Türkiston: `#005588` wird zu `#058`. 
- `rgb(0, 0, 128)`: Die dezimale Farbdefinition funktioniert im Prinzip wie die hexadezimalen Farbdefinition und bestimmt den Rot-, Grün- und Blauanteil einer Farbe von 0 bis 255. Aus dem hexadezimalen Wert `80` wird ind dieser Definition der dezimale Wert `128`.
- `rgba(0, 0, 128, 0.5)`: Die dezimale Farbdefinition hat noch einen vierten Parameter der die Transparenz einer Farbe bestimmt. `0` ist durchsichtig, `1` ist undurchsichtig.

📖 **MDN**: [Farben](https://developer.mozilla.org/en-US/docs/Web/CSS/Farben)
