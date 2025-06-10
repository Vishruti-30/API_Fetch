# 🌦️ Weather Data Collector using OpenWeatherMap API

This project is a simple Python script that fetches real-time weather data for multiple cities using the **OpenWeatherMap API** and saves the results into a structured JSON file.

## 🔍 Objective
To automate the collection of live weather data for a list of cities and store it in a machine-readable format (JSON) for further use in data analysis, dashboards, or weather monitoring tools.

## 📁 Output
- `weather_data.json`: A JSON file containing weather metrics (temperature, humidity, wind speed, and description) for each city in the list.

## 🌐 API Details
- **Provider**: [OpenWeatherMap](https://openweathermap.org/api)
- **Endpoint Used**: `https://api.openweathermap.org/data/2.5/weather`
- **Data Points**:
  - Temperature (°C)
  - Weather Description
  - Humidity (%)
  - Wind Speed (m/s)

## 🛠️ Tools & Technologies
- **Python 3**
- **Requests** library for API calls
- **JSON** module for file creation

## 🏙️ Cities Included
- Toronto  
- New York  
- London  
- Paris  
- Tokyo

> You can easily modify the city list in the script to include any location of your choice.

## 🧾 Sample Output (JSON Format)
```json
{
    "Toronto": {
        "temperature": 17.4,
        "description": "few clouds",
        "humidity": 81,
        "wind_speed": 8.05
    },
    "New York": {
        "temperature": 19.6,
        "description": "clear sky",
        "humidity": 70,
        "wind_speed": 6.3
    }
}
```

## 🧩 How It Works
1. Define a list of cities to monitor
2. Loop through each city and call the OpenWeatherMap API
3. Parse the required weather fields
4. Store all results in a Python dictionary
5. Export the dictionary to `weather_data.json`


## 📦 File Structure
```
weather-api-project/
│
├── weather_data.py   # Main script
└── weather_data.json      # Output file (generated after run)
```

## 🚀 Future Enhancements
- 🌍 Add support for country codes and coordinates (lat/lon)
- 📅 Log historical data for time-series tracking
- 📊 Create a dashboard to visualize weather trends
- 📫 Schedule periodic data collection using CRON or Task Scheduler
