# Web-APIs

Web-APIs (Application Programming Interfaces) sind Schnittstellen, die vom Browser bereitgestellt werden, um bestimmte Funktionalitäten wie Geolokalisierung, Kamera- oder Dateien-Zugriff zu ermöglichen. Diese Funktionalitäten können direkt aus JavaScript heraus verwendet werden.

Ein einfaches Beispiel für die Verwendung einer Browser-API ist die Ermittlung des Standorts eines Benutzers. Hierfür kann die Geolocation-API verwenden werden:

```javascript
<script>
  if (navigator.geolocation) {
    navigator.geolocation.getCurrentPosition(function(position) {
      console.log('Latitude: ' + position.coords.latitude);
      console.log('Longitude: ' + position.coords.longitude);
    });
  } else {
    console.log('Geolokalisierung wird von diesem Browser nicht unterstützt.');
  }
</script>
```

In diesem Beispiel wird zuerst überprüft, ob der Browser die Geolokalisierung unterstützt. Falls ja, wird mit `navigator.geolocation.getCurrentPosition` der Standort des Benutzers abgefragt. Die Funktion, die hier als Argument übergeben wird, wird aufgerufen, wenn die Geolokalisierung erfolgreich ermittelt wurde. In dieser Funktion werden dann Längen- und Breitengrad auf der Browser-Konsole ausgegeben.

💡 _Es ist wichtig zu beachten, dass manche Browser APIs nur dann zur Verfügung stehen, wenn die Webseite über eine gültige SSL-Zertifizierung verfügt und sicher über HTTPS aufgerufen wird. Außerdem kann es sein, dass der Benutzer der Verwendung bestimmter APIs erst einmal genehmigen muss._

Browser APIs ermöglichen es, die Funktionalitäten des Browsers direkt von JavaScript aus zu nutzen und interaktive Webseiten zu erstellen, die besser auf die Bedürfnisse des Benutzers eingehen.

📖 **MDN**: [Introduction to Web APIs](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Introduction)
