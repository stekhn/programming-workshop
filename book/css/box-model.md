### Box-Model
Das CSS-Boxmodell ist die Grundlage für das Layout im Web. Jedes Element wird als rechteckige Box dargestellt. Jedes Element kann einen Innenabstand (*padding*), einen Rahmen (*border*) und einen Außenabstand (*margin*) haben. Diese Werte ergeben zusammen mit der intrinsischen Höhe/Breite die absolute Höhe/Breite eines Elements:

```         
+-----------------------------------------------------------------+
|                             margin                              |
|    +-------------------------------------------------------+    |
|    |                        border                         |    |
|    |    +---------------------------------------------+    |    |
|    |    |                   padding                   |    |    |
|    |    |    +-----------------------------------+    |    |    |
|    |    |    |              element              |    |    |    |
|    |    |    |                                   |    |    |    |
|    |    |    |                                   |    |    |    |
```

Als Beispiel dient hier eine Container für eine Infobox:

```html
<section class="info-box">
  <p>Eine Absatz mit informativem Inhalt</p>
</section>
```

Die Breite des Containers wird auf 100% der Seitenbreite gesetzt. Die Höhe wird nicht gesetzt und daher von der Größe des Inhalts (viel Text, wenig Text) bestimmt. Außerdem bekommt der Container einen Außenabstand, einen farbigen Rand und Außenabstand von jeweils `20px`. 

```css
.info-box {
  width: 100%;
  margin: 20px;
  padding: 20px;
  border: 20px solid red;
}
```
