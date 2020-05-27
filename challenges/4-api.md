# API-Aufgabe

In dieser Aufgabe geht es darum eine API anzuzapfen. Dafür verwenden wir die [API von OpenWeatherMap](https://openweathermap.org/api), welche weltweit aktuelle Wetterdaten liefert.

Auf unsere Infoseite zum Leben der Schwarzfußkatze wollen wir einen aktuellen Wetterbericht einblenden, damit unsere Benutzer sehen können ob die Kätzchen gerade in der Sonne baden oder frieren müssen.

Die API wird über eine URL mit bestimmten Parametern angefragt und ist folgendermaßen aufgebaut:

- `https://api.openweathermap.org/data/2.5/weather`: URL des API-Endpunkts
- `q=Upington,ZA`: Suchbegriff für den Ort für den wir das Wetter wissen wollen
- `units=metric`: Format in dem wir die Wetterdaten haben wollen (Grad Celsius)
- `appid=86573a082f27e2374ef4541a388c0311`: Steffens persönlicher Benutzerschlüssel

Zusammen sieht das so aus: `https://api.openweathermap.org/data/2.5/weather?q=Upington,ZA&units=metric&appid=86573a082f27e2374ef4541a388c0311`

Zurück bekommen wir eine JSON-Objekt mit folgenden Werten:

```json
{
  "coord": {
    "lon": 21.24,
    "lat": -28.46
  },
  "weather": [
    {
      "id": 800,
      "main": "Clear",
      "description": "clear sky",
      "icon": "01n"
    }
  ],
  "base": "stations",
  "main": {
    "temp": 18,
    "pressure": 1021,
    "humidity": 31,
    "temp_min": 18,
    "temp_max": 18
  },
  "visibility": 10000,
  "wind": {
    "speed": 1.5,
    "deg": 150
  },
  "clouds": {
    "all": 0
  },
  "dt": 1557421200,
  "sys": {
    "type": 1,
    "id": 1990,
    "message": 0.0043,
    "country": "ZA",
    "sunrise": 1557378378,
    "sunset": 1557417403
  },
  "id": 945945,
  "name": "Upington",
  "cod": 200
}
```

Da das Anfragen von Daten nicht ganz einfach ist, habe ich euch eine Funktion gebaut, welche sich darum kümmert die Daten von der API-Schnittstelle abzuholen. Was ihr mit den Daten macht, müsst ihr entscheiden.

```javascript
getWeather('Upington')
  .then(setWeather);

function setWeather(data) {
  // Hier könnt ihr mit den Daten arbeiten
}

async function getWeather(city) {
  const response = await fetch(`https://api.openweathermap.org/data/2.5/weather?q=${city}&units=metric&lang=de&appid=86573a082f27e2374ef4541a388c0311`);
  return await response.json();
}
```
