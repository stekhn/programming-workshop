# Float

Die `float`-Eigenschaft ermöglicht es Bilder und Textblöcke aus dem Textfluss herauszunehmen und nach links oder rechts zu verschieben. Die Methode ist nur schlecht dazu geeignet aufwendige, mehrspaltige Seitenlayouts zu bauen. Hierfür sollte man immer Flexbox oder Grid verwenden.

Das folgende Beispiel zeigt einen Zitatkasten, welchen wir nach rechts verschieben wollen („ausblocken“). Außerdem folgen drei Absätze Blindtext, um den Effekt von `float` zu verdeutlichen:

```html
<section class="quote">
  <p>„Ein tiefgründiges Zitat zum Zustand der Welt“</p>
</section>

<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla luctus aliquam dolor, eu lacinia lorem placerat vulputate. Duis felis orci, pulvinar id metus ut, rutrum luctus orci. Cras porttitor imperdiet nunc, at ultricies tellus laoreet sit amet. </p>
    
<p>Sed auctor cursus massa at porta. Integer ligula ipsum, tristique sit amet orci vel, viverra egestas ligula. Curabitur vehicula tellus neque, ac ornare ex malesuada et. In vitae convallis lacus. Aliquam erat volutpat. Suspendisse ac imperdiet turpis. Aenean finibus sollicitudin eros pharetra congue. Duis ornare egestas augue ut luctus. Proin blandit quam nec lacus varius commodo et a urna. Ut id ornare felis, eget fermentum sapien.</p>

<p>Nam vulputate diam nec tempor bibendum. Donec luctus augue eget malesuada ultrices. Phasellus turpis est, posuere sit amet dapibus ut, facilisis sed est. Nam id risus quis ante semper consectetur eget aliquam lorem. Vivamus tristique elit dolor, sed pretium metus suscipit vel. Mauris ultricies lectus sed lobortis finibus.</p>
```

Die halbe Breite sorgt dafür, dass der übrige Text den Zitatkasten umfließen kann. Eine größere Schrift und die Hintergrundfarbe helfen dabei, denn Zitatkasten hervorzuheben:

```css
.info-box {
  float: right;
  width: 50%;
  margin: 20px;
  font-size: 2em;
  background-color: lightgray;
}
```

📖 **MDN**: [Floats](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Floats)
