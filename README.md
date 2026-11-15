<div align="center">

# 🌱 Bodoor
### Cloud & IoT Platform for Sustainable Smart Irrigation

*Every drop of water and every kilowatt of solar energy, used efficiently.*

![Hackathon](https://img.shields.io/badge/Hackathon-Top%203%20Winner-brightgreen)
![Frontend](https://img.shields.io/badge/Frontend-HTML5%20%7C%20CSS3%20%7C%20Bootstrap%205-blue)
![IoT](https://img.shields.io/badge/IoT-ESP32%20%7C%20LoRaWAN%20%7C%20MQTT-orange)
![Backend](https://img.shields.io/badge/Backend-Laravel-red)

</div>

> 🏆 **Top 3 Winning Project: Hackathon "Act for AgWater Souss-Massa" (December 2024)**  
> *Organized by AgriEdge, Université Ibn Zohr, Enactus Morocco, and Cité de l'Innovation Souss-Massa (CISM).*

---

## Table of Contents
- [Vision & Mission](#-vision--mission)
- [The Problem We Solve](#-the-problem-we-solve)
- [Our End-to-End Solution](#-our-end-to-end-solution)
- [Key Dashboard Features](#-key-dashboard-features)
- [Tech Stack & System Architecture](#-tech-stack--system-architecture)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started-local-preview)
- [Target Ecosystem & Partners](#-target-ecosystem--partners)
- [Team](#-team-bodoor)
- [License](#-license)

---

## 🌍 Vision & Mission

**Bodoor** is an integrated Cloud and IoT solution designed to optimize agricultural water and energy usage from a sustainable and ecological perspective.

In regions facing severe water scarcity, traditional irrigation often relies on guesswork rather than real-time field data. Our vision is to empower farmers and agricultural cooperatives with accessible, data-driven precision agriculture tools, bridging low-power IoT field sensors with an intuitive Arabic (RTL) web dashboard so that every drop of water and every kilowatt of solar energy is used efficiently.

---

## ❓ The Problem We Solve

Agricultural water management currently faces two critical operational challenges:
1. **Suboptimal irrigation scheduling:** farmers often lack accurate, real-time insights into the exact volume of water their crops require and the ideal time to irrigate.
2. **Undetected water leaks:** when pipeline or drip-system leaks occur, farmers cannot quickly pinpoint their exact location.

Together, these blind spots lead to significant water wastage, higher energy costs, and reduced crop yield sustainability.

---

## 💡 Our End-to-End Solution

Bodoor combines connected hardware deployed directly in fields and greenhouses with a centralized cloud monitoring dashboard.

| Capability | Description |
| :--- | :--- |
| **Smart field sensing & actuation** | Connected nodes (ESP32 and long-range LoRaWAN transceivers) continuously measure soil moisture, water flow rate, pipeline pressure, water levels, and microclimate conditions (temperature, humidity, wind). Automated solenoid valves and smart pumps enable remote and threshold-based irrigation control. |
| **Accessible cloud dashboard (RTL)** | A clean Arabic Right-to-Left interface (`main-rtl`) ensures direct usability for local farmers and cooperative operators. |
| **Real-time anomaly & leak detection** | Instant visual alerts flag abnormal pressure drops or water leaks to prevent resource loss. |
| **Hybrid energy tracking** | Built-in telemetry tracks solar energy production, battery charge/discharge cycles, and grid import/export metrics alongside water consumption. |

---

## ✨ Key Dashboard Features

### 1. Water & Climate Telemetry (`index.html`)
- **Microclimate monitoring:** live tracking of ambient temperature (°C), air humidity (%), and wind speed (km/h).
- **Soil & irrigation gauges:** interactive gauges showing soil moisture percentage, evaporation rate ($\text{m}^3/\text{min}$), and daily irrigation flow ($\text{mm/day}$).
- **Leak alert system:** dedicated real-time status indicator for immediate water leak detection.
- **Historical analytics:** multi-year water consumption trend charts (2018–2024) for seasonal planning and reporting.

### 2. Energy & Equipment Performance (`performance.html`)
- **Solar & grid balance:** live monitoring of solar energy generation, home/farm load, battery charge levels, and net grid import/export.
- **Equipment breakdown:** distribution charts analyzing consumption across pumps, HVAC, lighting, and agricultural machinery.
- **Cost & tariff tracking:** automated calculation of imported/exported energy costs.

---

## 🛠️ Tech Stack & System Architecture

| Layer | Technologies |
| :--- | :--- |
| **Frontend UI** | HTML5, CSS3 / SCSS, Bootstrap 5 (`bs5`), JavaScript, RTL layout support |
| **Backend & Cloud** | Laravel, RESTful APIs |
| **IoT & Connectivity** | ESP32, LoRaWAN (E220-900T30D), MQTT protocol, Wi-Fi |
| **Field Hardware** | Soil moisture sensors, flow meters, pressure sensors, ultrasonic level sensors, DHT temperature/humidity sensors, solenoid valves, smart water pumps |

---

## 📂 Project Structure

```text
bs5/
├── assets/                     # Third-party libraries, icons, and chart plugins
├── images/                     # Logos, dashboard visuals, and favicon
└── template/
    └── vertical/
        ├── main-rtl/
        │   ├── index.html          # Main Water & Climate Monitoring Dashboard
        │   └── performance.html    # Solar & Energy Performance Dashboard
        └── src/
            ├── css/                # Compiled stylesheets (style.css, skin_color.css, custom.css)
            ├── js/                 # Dashboard interactivity and chart scripts
            └── scss/               # Source SCSS files
```

---

## 🚀 Getting Started (Local Preview)

1. **Clone the repository**
   ```bash
   git clone [https://github.com/monyaoubella93/Bodoor-AgWater-Dashboard.git](https://github.com/monyaoubella93/Bodoor-AgWater-Dashboard.git)
   cd Bodoor-AgWater-Dashboard
   ```
2. **Launch with a local server**
   - Open the project folder in **VS Code**.
   - Install the **Live Server** (or **Five Server**) extension.
   - Right-click `template/vertical/main-rtl/index.html` and select **Open with Live Server**.

---

## 🤝 Target Ecosystem & Partners

- **Target users:** individual farmers, agricultural cooperatives, and specialized agribusinesses.
- **Strategic ecosystem:** agricultural cooperatives (for field testing and adoption), smart sensor and pump suppliers, and public institutions / NGOs supporting sustainable agriculture.

---

## 👥 Team Bodoor

Developed with passion during the **AgWater Souss-Massa Hackathon (December 6–7, 2024)**:
- **Monya Oubella**
- **Sara Daoudi**
- **Badreddine Ouajih**
- **Ayoub Elbouzari**
- **Ikram Elaima**

---

## 📄 License

This project was created as an academic and hackathon innovation prototype. Feel free to explore the codebase or reach out for collaboration opportunities.