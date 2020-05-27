# Programmieren für Journalisten

Programmiersprachen sind die flexiblesten Werkzeuge, die der Mensch jemals entwickelt hat. Sie helfen uns zeitraubende Aufgaben zu automatisieren und komplexe Probleme zu lösen. Egal ob Smartphone, Waschmaschine oder Ampelanlage, mittlerweile wird unser Leben an vielen Stellen von Software bestimmt. Programmieren zu lernen, hilft dabei eine zunehmend digitale Welt besser zu verstehen.

Gerade für Journalisten ist diese Verständnis zunehmend wichtig, um kritisch über Herausforderungen und Probleme zu berichten, die durch die Digitalisierung unserer Gesellschaft entstehen. Außerdem können Journalisten selbst Methoden und Werkzeuge aus der Softwareentwicklung nutzen, um Geschichten in großen Datensätzen finden und interaktiv für die Veröffentlichung online aufzubereiten.

Glücklicherweise ist Programmieren lernen so einfach wie noch nie und erfordert vor allem Spaß am Lernen und Ausprobieren.

**Die Inhalte des Seminars gibt es hier als kostenloses, digitales Buch:**  
<https://stekhn.github.io/programming-workshop/>

## Ziel des Seminars

Teilnehmer des Seminars sollen die Grundlagen der Web-Entwicklung mit HTML, CSS und JavaScript lernen. Dabei steht die praktische Vermittlung von Programmierkenntnissen, so wie das Entwickeln von Problemlösungsstrategien im Vordergrund.

## Seminarunterlagen

Das Seminar besteht aus mehrere Blöcken mit Präsentationen, Aufgaben und Diskussion. Die Inhalte der einzelnen Blöcke sind alle frei zugänglich.

- [Seminarinhalte](https://stekhn.github.io/programming-workshop/)
- [Präsentation](https://github.com/stekhn/programming-workshop/blob/master/slides.pdf)
- [Aufgaben](https://github.com/stekhn/programming-workshop/tree/master/challenges)
- [Lösungen](https://github.com/stekhn/programming-workshop/tree/master/solutions)

## Dokumentation erstellen

Die [Dokumentation](https://stekhn.github.io/programming-workshop/) wurde mit [mdBook](https://github.com/rust-lang/mdBook) erstellt. mdBook ist ein Programm zum Erstellen von digitalen Büchern aus Markdown-Dokumenten. Die Markdown-Dokumente liegen im Ordner `book`. Die draus erstellte Dokumentation liegt im Ordner `docs` und wird über Github Pages ausgeliefert.

Um mdBooks zu installieren, muss [Rust](https://www.rust-lang.org/) und [Cargo](https://doc.rust-lang.org/cargo/) installiert sein. Danach kann mdBook über die Kommandozeile installiert werden:

```console
cargo install mdbook
```

Dokumentation einmalig neu erstellen:

```console
mdbook build
```

Dokumentation bei Änderungen neu bauen und über `http://localhost:3000/` bereitstellen:

```console
mdbook serve
```

Die Grundeinstellungen des Buchs finden sich in `book.toml`, das Inhaltsverzeichnis in `book/SUMMARY.md`.
