# Flight Passport

<p align="right">
  <strong>English</strong> | <a href="README_CN.md">简体中文</a>
</p>


Flight Passport is a minimalist, serverless flight journal and Web-GIS tracker designed to visualize personal aviation history with absolute elegance. Built entirely within a single-file architecture, this application strips away the modern bloat of heavy front-end frameworks and complex build tools, returning to the clean efficiency of vanilla JavaScript and pure CSS orchestration.

### The Philosophy of Zero-Friction

Modern Web-GIS development is increasingly constrained by corporate API gateways, requiring credit card bindings and tracking tokens just to render a basic basemap. Flight Passport breaks this dependency chain. By interacting directly with open Google Maps XYZ tile streams, the application delivers both high-fidelity standard rendered maps and raw hybrid satellite imagery without requiring any API keys or registration. This approach ensures that your flight journal remains permanently portable, completely private, and deployable in any offline or air-gapped environment.

### Cartographic Duality and Geodesic Truth

The core technical narrative of Flight Passport lies in its real-time projection switching, which visualizes the inherent tension between the curved Earth and flat digital screens:

* **Spherical Great Circle Mode** calculates the true physical trajectory of flight. It implements geodetic interpolation to project the shortest distance on a sphere onto the Web Mercator canvas, resulting in the organic, sweeping arcs characteristic of real-world aviation paths.
* **Planar Mercator Mode** operates in pure screen-space coordinates. It linearizes the path between coordinates to present straight lines across the projection plane, reflecting the classic, structural aesthetics of traditional flat paper charts.

By handling multiple overlapping routes between identical city pairs, the mathematical engine automatically introduces dynamic offset curves, preventing visual collision and maintaining structural clarity even within dense global flight networks.

### Architecture and Local Autonomy

The interface follows a strict local-first data model. Your complete flight log, airport metrics, and historical statistics reside entirely inside your browser localized web storage. No external servers are contacted; no data leaves your machine. 

To maintain visual cohesion with contemporary dark-themed interfaces, the mapping engine applies real-time CSS matrix filtration directly onto the map canvas. In rendered mode, the tiles undergo a precise hue-rotation, inversion, and brightness adjustment to create a sci-fi cyber-cartography theme. When switched to satellite mode, the filter instantly disengages, preserving the rich, unaltered natural biomes of the earth.

### Instant Deployment

To launch your personal journal, simply download the `flight_passport.html` file and execute it in any modern browser. The application automatically pulls the required lightweight mapping library via secure content delivery networks and instantiates the global workspace immediately.