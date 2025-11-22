# 🏎️ F1 Live Dashboard — Desktop App (Electron + OpenF1)

A modern, beautifully designed Formula 1 live dashboard and season history viewer, powered by the **OpenF1 API**, packaged as a **desktop application** using **Electron**.

This app provides:

- Live timing tower  
- Driver gaps, last laps, and lap counts  
- Race control messages (flags, incidents, steward decisions)  
- Weekend schedule  
- Auto-detect race weekends  
- Weather forecast for the next venue  
- Animated F1 race-start lights  
- Season history (auto-detected year)  
- Dark/light mode  
- Windows `.exe` installer (via Electron Builder)  

---

## 🚀 Features

### 📡 **Live Dashboard**
- Timing tower with positions, gaps, laps, and team colors  
- Race control messages (live updates)  
- Live weekend info: session, location, schedule  
- Auto-refresh data  
- Modern UI with light/dark themes  

### 🕒 **Pre-Race / Off-Weekend History Page**
- F1-style animated race lights  
- Countdown to next official session  
- Season history auto-detected from the latest available year  
- Weather for the next race venue  
- Smooth page transitions  

### 📦 **Desktop App**
- One-click Windows installer (`setup.exe`)  
- Auto-launches internal API proxy (Express server)  
- Opens the live dashboard inside Electron  
- Custom **F1 icon** included  

---

F1 Live Dashboard Setup.exe


### **2. Install**
Double-click the installer:



dist/F1 Live Dashboard Setup X.X.X.exe


This installs the app into Windows (Start Menu entry included).

### **3. Launch**
Open from:



Start Menu → F1 Live Dashboard


The app automatically:

- Starts its internal Express proxy (`http://localhost:5000`)
- Loads the UI (`index.html`)
- Fetches OpenF1 data

---

# 🔧 Development Setup (Run from Source)

### **1. Clone the repo**

```bash
git clone https://github.com/YOUR_USERNAME/f1-live-dashboard.git
cd f1-live-dashboard


🌐 Why a Local Proxy?

OpenF1 occasionally blocks direct browser requests due to CORS and rate limits.

To ensure stability, this app uses a local proxy server:

http://localhost:5000/api


which forwards all traffic to:

https://api.openf1.org/v1


This ensures:

No CORS issues

Reliable data

Fast local caching

Works inside Electron

🛠️ Technologies Used

Electron – Desktop application

Express.js – Local API proxy

OpenF1 API – Session & timing data

Open-Meteo API – Weather forecasts

HTML / CSS / JavaScript – UI

Electron Builder – Packaging & installer

⚠️ Disclaimer

This project is unofficial and not affiliated with Formula 1, Liberty Media, or the FIA.
Data is provided by OpenF1, which aggregates public timing feeds.

For personal use only.

📄 License

Belongs to Shahzaib Khan (Thats me).

🏁 Enjoy the App!

If you'd like additional features:

Auto-update system

Custom splash screen

Real-time track map showing car positions

Team/driver themes

Mobile app version

Cloud data sync

Just open an issue or request enhancements!

Add your screenshots here once available.

