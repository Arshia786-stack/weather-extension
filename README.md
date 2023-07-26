# Weather Extension

This is a weather extension that allows users to retrieve the current weather and forecast for a specific city. The extension is implemented using HTML, CSS, and JavaScript, and it utilizes the OpenWeatherMap API to fetch weather data.

## Usage

1. Open the extension popup by clicking on the extension icon.
2. In the popup, enter the name of the city for which you want to retrieve the weather information.
3. Click the "Get Weather" button to fetch the current weather data for the specified city.
4. Click the "Forecast" button to retrieve the forecast for the specified city.
5. The weather details will be displayed in the "Weather Details" section, and the forecast will be displayed in the "Forecast Details" section.

## Files

- `index.html`: The main HTML file that defines the structure of the extension popup.
- `styles.css`: The CSS file that contains the styles for the extension popup.
- `popup.js`: The JavaScript file that handles the functionality of the extension.

## Dependencies

This extension requires an internet connection to fetch weather data from the OpenWeatherMap API. Additionally, it utilizes the following resources:

- OpenWeatherMap API: To fetch weather and forecast data.
- `temperature-icon.png`: An icon used to represent temperature in the weather details.
- `description-icon.png`: An icon used to represent the weather description in the weather details.
- `humidity-icon.png`: An icon used to represent humidity in the weather details.
- `wind-icon.png`: An icon used to represent wind speed in the weather details.

## Contributions

Contributions are welcome! If you have any ideas, suggestions, or improvements for the Weather Extension, please feel free to open an issue or submit a pull request.

## How It Works

- When the extension popup is opened, the JavaScript code in `popup.js` attaches event listeners to the "Get Weather" and "Forecast" buttons.
- When the "Get Weather" button is clicked, the `getWeather()` function is called, which retrieves the current weather data for the specified city using the OpenWeatherMap API.
- When the "Forecast" button is clicked, the `getForecast()` function is called, which retrieves the forecast data for the specified city using the OpenWeatherMap API.
- The fetched weather and forecast data are then passed to the `displayWeather()` and `displayForecast()` functions, respectively, which populate the respective sections in the popup with the received data.

## API Key

To use this extension, you need to obtain an API key from OpenWeatherMap and replace the `appid` parameter in the API URLs in `popup.js` with your own API key.
                                                       
                                                        Made with ❤️ by Arshia Mubias Shaik

For example: Make sure to replace YOUR_API_KEY with your actual API key provided by OpenWeatherMap.

```javascript
var url = 'https://api.openweathermap.org/data/2.5/weather?q=' + encodeURIComponent(cityName) + '&appid=YOUR_API_KEY&units=metric';


