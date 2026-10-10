### 🌐 Click Here for Live Demo on Netlify
https://drivesafe-ai-v10-0.netlify.app

# drivesafe-ai
# 🚗 DriveSafe AI v10.0 — Flagship Navigation & Safety Telemetry Engine

[![License: Proprietary](https://img.shields.io/badge/License-All%20Rights%20Reserved-red.svg)]()
[![Hackathon](https://img.shields.io/badge/Submission-Hackoverflow%2010.0-cyan.svg)]()
[![Routing Engine](https://img.shields.io/badge/Routing-OSRM%20Road%20Snap-emerald.svg)]()
[![Spatial API](https://img.shields.io/badge/Spatial-OpenStreetMap-blue.svg)]()

**DriveSafe AI** is an automotive navigation and real-time road safety telemetry platform engineered to reduce highway accidents and accelerate municipal infrastructure response. Built as a lightweight, zero-dependency client application, it combines real-time OSRM road snapping, automated speech and sonar proximity guidance, client-side pixel-matrix computer vision defect inspection, and live spatial emergency dispatch.

---

## 🌟 Key Capabilities

* **🛣️ OSRM Real-Road Snapping & Dynamic Rerouting:** Connects directly to the Open Source Routing Machine (OSRM) engine to snap vehicle movements to exact street geometries. Automatically detects off-route drift greater than 70 meters and recalculates safe road paths in real time.
* **🔊 Hazard Proximity Voice & Sonar Alerts:** Integrated Web Speech Synthesis and Web Audio API synthesizer deliver turn-by-turn voice warnings and sonar beeps when approaching logged road hazards (potholes, blackspots, unlit stretches).
* **👁️ Canvas Pixel-Matrix Computer Vision Inspector:** Analyzes uploaded road condition photos on an HTML5 offscreen canvas matrix (`getImageData()`). Measures mean RGB luminance, edge contrast roughness, and dark pit ratios to compute physical crater depth ($\text{cm}$) and collision threat scores ($1-10$).
* **🚨 Real OpenStreetMap Spatial SOS Radar:** Queries live OpenStreetMap spatial APIs around user coordinates to locate nearby named hospitals, trauma centers, and police stations. Instantly generates emergency WhatsApp broadcast pins containing exact Google Maps coordinates.
* **📊 Dynamic Real-Time Analytics Dashboard:** Real-time data pipeline powered by Chart.js that dynamically updates network node health, municipal turnaround repair metrics, and hazard distributions as users report incidents.
* **🪞 Windshield Mirror HUD Mode:** Vertically flips the application viewport for inverted display reflection on automobile windshields during night driving.

---

## 🛠️ Tech Stack & Architecture

| Component | Technology / API | Purpose |
| :--- | :--- | :--- |
| **Map Engine** | [Leaflet.js](https://leafletjs.com/) | Interactive vector map viewport & tile rendering |
| **Tile Layers** | Esri Dark Canvas / CartoDB / OSM | High-contrast automotive map tiles |
| **Road Routing** | [OSRM API](http://project-osrm.org/) | Real-road path snapping & routing vectors |
| **Geocoding** | Nominatim / BigDataCloud API | Reverse geocoding for sector and street address lookup |
| **Computer Vision** | HTML5 Canvas API (`getImageData`) | Pixel-matrix luminance and contrast matrix analysis |
| **UI Styling** | Tailwind CSS | Dark-mode automotive dashboard interface |
| **Analytics Engine** | Chart.js | Dynamic doughnut and line graph visualizations |
| **Data Persistence** | Web LocalStorage | Client-side database persistence |

---

## 🚀 Quick Start & Running Locally

DriveSafe AI runs natively in any modern web browser without requiring node build steps or backend servers.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_GITHUB_USERNAME/drivesafe-ai.git](https://github.com/YOUR_GITHUB_USERNAME/drivesafe-ai.git)
