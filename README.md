# ✈️ Flight Passport

<p align="right">
  <strong>English</strong> | <a href="README_CN.md">简体中文</a>
</p>


**Flight Passport** is a single-file, offline-first web application designed for aviation enthusiasts and travelers to track their flight history. It visualizes your routes on a global map with a sleek, dark "Sci-Fi" aesthetic.

No backend, no build tools, no installation—just open the HTML file in your browser.

### ✨ Features

*   **🗺️ Dual Map Styles**: Switch between **Google Roadmap** (stylized with a dark blue filter) and **Google Satellite Hybrid**.
*   **📐 Projection Modes**: Choose between **Great Circle** (realistic spherical arcs) and **Mercator** (straight planar lines).
*   **📊 Rich Statistics**: Automatically calculates total distance, number of flights, unique airports, countries visited, and estimated flight time.
*   **💾 Local Storage**: Your flight data is saved directly in your browser. It persists across sessions without a server.
*   **🌐 Global Coverage**: Pre-loaded with 150+ major airports worldwide (IATA codes included).

### 🚀 Getting Started

1.  **Download**: Clone this repository or download the `flight passport.html` file.
2.  **Open**: Double-click the file to open it in any modern browser (Chrome, Edge, Firefox recommended).
3.  **Network**: Ensure you have an internet connection for the Google Maps tiles to load.
4.  **Add Flights**: Enter IATA codes (e.g., `PVG` for Shanghai, `LAX` for Los Angeles) in the sidebar to start tracking.

### 🛠️ Tech Stack

*   **Frontend**: Vanilla JavaScript (ES6), HTML5, CSS3
*   **Mapping**: https://leafletjs.com/
*   **Tiles**: Google Maps (No API Key required for basic use via XYZ)

### 📝 Usage Notes

*   **IATA Codes**: The app uses 3-letter IATA codes. You can edit the `AIRPORTS` object in the `<script>` section to add more airports.
*   **Map Styling**: The "Standard Render" mode uses CSS `filter` (hue-rotate, invert) to create a dark theme that matches the UI. The "Satellite" mode displays real imagery.


### 🙏 Acknowledgement
This project is inspired by and references https://github.com/Airbus788/flight_passport. Special thanks to the original author!


### 🙏 致谢
本项目参考并借鉴了 https://github.com/Airbus788/flight_passport，特此致谢！
