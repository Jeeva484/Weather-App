# Weather App

A lightweight, responsive weather app that looks up current conditions by city using the OpenWeatherMap Current Weather API.

Live demo: <https://weather-app-cyan-nu-97.vercel.app/>

## Features

- Search by city name or press Enter.
- Current temperature, humidity, and wind speed.
- Weather-specific SVG icons with a fallback for other conditions.
- Clear messages for missing/invalid API keys, unknown cities, and connection failures.

## Run locally

1. Get an API key from [OpenWeatherMap](https://openweathermap.org/api).
2. From this folder, start a local static server:

   ```sh
   python3 -m http.server 8000
   ```

3. Open <http://localhost:8000>, expand **API key settings**, and save your key in this browser.

The key is stored in this browser's local storage and is not included in the project files. This is a static client-side app, so the key is still sent to the weather service from the browser and can be inspected by the browser user. Restrict its usage and quota in your OpenWeatherMap account; use a backend proxy if the key must remain private.

## Project structure

```text
.
├── README.md
├── images/
│   ├── clear.svg
│   ├── clouds.svg
│   ├── drizzle.svg
│   ├── humidity.svg
│   ├── mist.svg
│   ├── rain.svg
│   ├── search.svg
│   ├── snow.svg
│   ├── thunderstorm.svg
│   └── wind.svg
├── index.html
└── weather.css
```
