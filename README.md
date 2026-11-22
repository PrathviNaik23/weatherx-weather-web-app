# 🌤️ WeatherX — Smart Weather Dashboard

A modern and responsive **real-time weather web application** built using **HTML, CSS, and JavaScript**. WeatherX allows users to search for cities and retrieve live weather information through a REST API.

The application provides a clean glassmorphism-style dashboard with animated backgrounds, weather icons, quick city search, loading indicators, and error handling.

## 🚀 Features

- 🌍 Search weather by city name
- ⚡ Fetch real-time weather data using an API
- 🌡️ Display current temperature
- 💨 Display wind information
- ☁️ Display weather condition
- 🕐 Display the latest update time
- 📅 Display the current date
- 🌧️ Dynamic weather icons based on conditions
- 🔍 Search using button or Enter key
- 🏙️ Quick-access cities
- ⏳ Loading animation while fetching data
- ❌ Error handling for invalid/unavailable cities
- 📱 Responsive design for mobile, tablet, and desktop
- ✨ Animated gradient background
- 💎 Glassmorphism weather card

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Web page structure |
| CSS3 | Styling, animations and responsive design |
| JavaScript | Application logic and DOM manipulation |
| Fetch API | Fetching weather data |
| REST API | Real-time weather information |

## 🌐 API Used

WeatherX uses the **GoWeather API** to retrieve weather information.

The application sends a request based on the city entered by the user:

```javascript
fetch(`https://goweather.xyz/v2/weather/${city}`)
```

The API response is then converted into JSON and displayed dynamically on the dashboard.

## 🔄 How the Application Works

```text
                ┌──────────────────┐
                │   Enter City     │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │ JavaScript Gets   │
                │   City Name       │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │   Fetch API       │
                │  Weather Data     │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │   JSON Response   │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │ Process Weather   │
                │      Data         │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │ Update Dashboard  │
                └──────────────────┘
```

## 🖥️ Dashboard

The WeatherX dashboard displays:

- City name
- Current temperature
- Weather description
- Wind information
- Temperature statistics
- Weather condition
- Current update time
- Current date
- Dynamic weather icon

The weather information is updated dynamically after the API response is received.

## 🏙️ Quick City Search

WeatherX provides predefined quick-search cities:

- Bengaluru
- Mumbai
- Delhi
- London
- New York

Users can select a city without manually typing it into the search box.

## 🎨 UI & Design

The application uses a modern dashboard design featuring:

- Glassmorphism cards
- Gradient background
- Animated floating background elements
- Smooth hover effects
- Responsive layouts
- Animated weather icons
- Loading spinner
- Modern search interface

The main interface uses a dark gradient background with blue and purple visual effects.

## 📱 Responsive Design

WeatherX is designed to work across different screen sizes.

### Desktop

The weather statistics are displayed in a four-column layout.

### Tablet

The statistics adapt into a two-column layout.

### Mobile

The search interface becomes vertically stacked and the weather card adjusts its spacing and typography for smaller screens.

## ⚠️ Error Handling

The application handles situations such as:

- Empty city search
- Failed weather API requests
- Invalid/unavailable city information

An error message is displayed to the user instead of allowing the application to fail silently. 

## ⏳ Loading State

While weather information is being retrieved, WeatherX displays a loading spinner and temporarily reduces the weather card opacity.

This gives the user visual feedback that the API request is in progress.

## 🌦️ Dynamic Weather Icons

WeatherX automatically selects an emoji based on the weather description.

For example:

```text
Rain      → 🌧️
Cloud     → ☁️
Storm     → ⛈️
Snow      → ❄️
Sun       → ☀️
Other     → 🌤️
```

The application checks the weather description returned by the API and dynamically changes the displayed icon.

## 📂 Project Structure

```text
WeatherX/
│
├── index.html
└── README.md
```

> The current version contains the HTML, CSS, and JavaScript in a single `index.html` file.

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/weatherx.git
```

### 2. Open the project

```bash
cd weatherx
```

### 3. Run the application

Open `index.html` in your browser.

You can also use **VS Code + Live Server** for easier development.

## 🔍 Example

Enter a city such as:

```text
Bengaluru
```

Then click:

```text
🔍 Search
```

The application requests weather information from the API and updates the dashboard with the returned data.

## 📸 Screenshots

Add your project screenshots here:

```markdown
## 📸 Screenshots

![WeatherX Dashboard](screenshots/weatherx-dashboard.png)

![WeatherX Search](screenshots/weatherx-search.png)

![WeatherX Mobile](screenshots/weatherx-mobile.png)
```

Recommended screenshots:

1. Main dashboard
2. Weather search result
3. Quick city search
4. Mobile responsive view
5. Error message

## 🎯 Project Objectives

This project was developed to practice and demonstrate:

- REST API integration
- JavaScript Fetch API
- `async` data handling
- JSON data processing
- DOM manipulation
- Event handling
- Responsive web design
- Error handling
- Dynamic UI updates

## 📚 What I Learned

Through this project, I practiced:

- How to consume an external API
- How to use JavaScript `fetch()`
- How to process JSON responses
- How to dynamically update HTML elements
- How to handle API errors
- How to create responsive layouts
- How to create interactive web interfaces
- How to build a real-world API-based project

## 🔮 Future Improvements

Possible future enhancements include:

- 📍 Current-location weather
- 📅 5-day weather forecast
- 🌡️ Celsius/Fahrenheit conversion
- 🌙 Dark/light theme switcher
- ⭐ Favorite cities
- 🌍 More detailed location information
- 📊 Weather charts
- 🌅 Sunrise and sunset information
- 📈 Historical weather data

## 👨‍💻 Author

**Prathvi**

BCA Graduate | Fresher

### Areas of Interest

- Data Analytics
- Data Science
- AI/ML
- Python
- Web Development

## ⭐ Support

If you like this project, consider giving the repository a ⭐ on GitHub.

---

**WeatherX — Real-time weather information with a modern web experience.**
