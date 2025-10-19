# 🌦️ React Weather-App

A simple and beautiful Weather Application built with React.js and the OpenWeather API.
The app allows users to search for the current weather in any city and displays the temperature, weather condition, and the date with a dynamic background that changes based on the temperature.

---

## 🚀 Features

🌍 Search for real-time weather data by city name

🌡️ Displays temperature in °C and current weather condition

🕒 Shows current date and day dynamically

🌤️ Background image changes depending on the temperature (warm or cold)

⚡ Instant weather updates with Enter key

💻 Fully responsive and simple UI
---
## 🧰 Tech Stack

React.js ⚛️

OpenWeather API 🌦️

CSS / TailwindCSS 💅

JavaScript (ES6+)

```
📂 Project Structure
weather-app/
│
├── public/
│   └── index.html
│
├── src/
│   ├── assets/
│   │   ├── cold-bg.jpg
│   │   └── warm-bg.jpg
│   ├── App.jsx
│   ├── App.css
│   └── main.jsx
│
├── package.json
├── vite.config.js
└── README.md
```
## 🧭 How It Works

User types a city name in the input field.

When the Enter key is pressed, the app triggers the search function.

It calls the OpenWeather API with the provided city name.

### The app displays:

City name and country

Current temperature (in °C)

Weather condition (e.g., Clear, Clouds, Rain)

Current date

If the temperature is above 16°C, the background changes to a warm image. Otherwise, a cold image is shown.

## 🔑 API Setup

Go to OpenWeather API
 and create a free account.

Generate your API key.

Replace the placeholder in App.jsx:
```
const api = {
  key: "YOUR_API_KEY",
  base: "https://api.openweathermap.org/data/2.5/"
};
```
## 🛠️ Installation & Setup

Clone the repository

git clone https://github.com/your-username/weather-app.git


Navigate to the project folder

cd weather-app


Install dependencies

npm install


Run the development server

npm run dev


Open your browser and go to: http://localhost:5173

## 🧊 Styling & UI

The app uses background images to reflect warm and cold weather.

Responsive and clean layout.

Weather details are centered for better visibility.

.app {
  background-image: url('./assets/cold-bg.jpg');
}

.app.warm {
  background-image: url('./assets/warm-bg.jpg');
}

```
📸 Sample UI
---------------------------------
|  🌤️  London, GB               |
|  Tuesday 22 October 2025     |
|                               |
|           23°C               |
|          Clear Sky           |
---------------------------------
```
### ⚠️ Common Issues and Solution

❌ Error: “API key is missing” → Ensure your key is correctly added in App.jsx.

❌ Background not changing → Check if the temperature threshold and class names match (app and app warm).

❌ No response from API → Confirm that the API endpoint is correct:

https://api.openweathermap.org/data/2.5/

## 📄 License

This project is licensed under the MIT License.

## 🙌 Acknowledgements

OpenWeather API
 for providing weather data

React.js
 for the frontend framework

Vite
 for fast development

✅ Author: @kudostech

💻 Portfolio: https://kudostech-portfolio-website.vercel.app
