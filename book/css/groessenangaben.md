# Größenangaben

In CSS gibt es verschiedene Arten Größenangaben zu definieren. Um Layouts genau umzusetzen und leicht anpassbar zu entwickeln, ist es wichtig die unterschiede zwischen den verschiedenen Einheiten zu verstehen.

- `px`: Pixel ist die einfachste, aber auch unflexibelsten Einheit, welche man meistens eher vermeiden sollte. Diese liegt vor allem daran, dass jeder Benutzer vor einen unterschiedlich großen Bildschirm sitzt und es schwer ist für jede Konstellation die richtige Pixelgröße zu finden.
- `%`: Prozentangaben sind flexibel und vor allem für Größenangaben bei Bildern, Containern und Spalten geeignet 
- `em`: Eine beliebte relative Größenangaben die meisten für alles verwendet wird, was irgendwie mit Typografie zusammenhängt: Schriftgröße, Durchschuss, Abstände etc.
- `rem`: Funktioniert wie `em`, nur dass sich `rem` immer auf die (Schrift-)größe des `<body>`-Elements bezieht, während sich `em` immer auf die (Schrift-)größe des Elternelementes (*parent*) bezieht.
- `vh` und `vw`: Eine weiter relative Größeangabe, welche sich auf die Höhe des Benutzerbildschirms (`vh`) oder die Breite (`vw`) bezieht. Sehr praktisch für Aufmacherbilder und Container.

Außerdem gibt es die Einheiten `pc` (Pica) und `pt` (Punkt), welche aus den Urzeiten des Schriftsetzenwesens kommen und im modernen Webdesign eigentlich keine Relevanz mehr haben. 

📖 **W3C**: [CSS-Einheiten](https://www.w3.org/Style/Examples/007/units.de.html)
