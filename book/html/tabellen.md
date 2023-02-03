# Tabellen

Tabellen sind nützliche Helfer um Daten und Informationen strukturiert darzustellen. Eine Tabelle besteht immer aus mehreren verschachtelten HTML-Elementen:

- `<table>`: Markiert eine Tabelle, d.h. Daten mit mehr als einer Dimension.
- `<tr>`: Steht für eine Zeile mit Tabellenzellen.
- `<td>`: Kennzeichnet eine einzelne Tabellenzelle.
- `<th>`: Kennzeichnet eine Tabellenzelle mit einer Beschriftung.

Diese zusätzliche Elemente helfen dabei die Tabelle inhaltlich zu strukturieren, sind aber nicht zwingend notwendig:

- `<tbody>`: Steht für die Spalten, die die eigentlichen Daten einer Tabelle enthalten.
- `<thead>`: Markiert die Gruppe der Tabellenzeilen, die die Beschriftungen der Tabellenspalten enthalten.
- `<tfoot>`: Markiert die Gruppe der Tabellenzeilen, die die Zusammenfassungen der Tabellenspalten enthalten.

Ein Beispiel für eine dreispaltige Tabelle mit vier Zeilen:

```html
<table>
  <tr>
    <th>Vorname</th>
    <th>Nachname</th>
    <th>Alter</th>
  </tr>
  <tr>
    <td>Philipp</td>
    <td>Primus</td>
    <td>25</td>
  </tr>
  <tr>
    <td>Oskar</td>
    <td>Optimus</td>
    <td>27</td>
  </tr>
  <tr>
    <td>Marlene</td>
    <td>Maximus</td>
    <td>22</td>
  </tr>
</table>
```

Daraus entsteht folgende Tabelle:

| Vorname | Nachname | Alter |
| ------- | -------- | ----- |
| Philipp | Primus   | 25    |
| Oskar   | Optimus  | 27    |
| Marlene | Maximus  | 22    |

> 💡 _HTML-Tabellen können auch mit dem praktischen [Tables Generator](https://www.tablesgenerator.com/html_tables) online erstellt werden._

📖 **MDN**: [Table Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/table)
