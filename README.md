# CarSpotter
CarSpotter is a mobile-first web app for tracking, valuing, and competing your real-world car sightings. Log cars into runs, track total value, build a personal garage, and sync everything across devices using Firebase.
# 🚗 CarSpotter

CarSpotter is a mobile-first Progressive Web App (PWA) designed for car enthusiasts who want to track, value, and compete their real-world car sightings.

Instead of just spotting cars, CarSpotter turns it into a game:

* Build "runs" of cars you see
* Track total value of each run
* Compete against your personal best
* Store every car in your garage
* Sync everything across devices

---

## ⚡ Features

### 🛣️ Run System

* Add cars to a **current run**
* Each car includes:

  * Name (Make/Model)
  * Estimated value
  * Color
  * Type (Supercar, Muscle, EV, etc.)
* Live total updates as you add cars
* Compare against your **best run**
* Save runs to history

### 👁️ Instant Spotting

* Log a car as **Spotted**
* Skips the run system entirely
* Saves directly to:

  * Garage
  * History

### 🏎️ Garage

* View all cars you've ever logged
* Stats include:

  * Total cars
  * Total value
  * Average value
* Sort by:

  * Value (high → low / low → high)
  * Alphabetical
* Click any car to search it instantly

### 📋 History

* Full log of:

  * All runs
  * Individual spotted cars
* Highlights:

  * Best run (record)
  * Run totals
  * Car breakdown per run

### ⚡ Quick Picks

* Automatically saves frequently logged cars
* Searchable dropdown for fast entry
* Speeds up logging significantly

### 🎤 Voice Notes

* Built-in notes system with:

  * Auto-save
  * Speech-to-text support (Web Speech API)
* Useful for quickly logging sightings without typing

### ☁️ Cloud Sync

* Powered by Firebase:

  * Authentication (Google Sign-In)
  * Firestore database
* Syncs:

  * Runs
  * Garage
  * Quick picks
  * Notes

### 💾 Backup & Restore

* Export your data as JSON
* Import backups anytime
* Merge local and cloud data safely

### 📱 PWA Support

* Installable on:

  * iPhone (Add to Home Screen)
  * Desktop (Chrome install)
* Works offline with service worker caching

---

## 🧠 How It Works

CarSpotter stores data in two main ways:

* **LocalStorage**

  * Fast access
  * Offline capability

* **Firebase Firestore**

  * Cross-device sync
  * Real-time updates

The app intelligently merges:

* Local data
* Cloud data
* Imported backups

---

## 🛠️ Tech Stack

* HTML, CSS, Vanilla JavaScript
* Firebase:

  * Authentication
  * Firestore
* Web APIs:

  * LocalStorage
  * Speech Recognition API
  * Service Workers (PWA)

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/carspotter.git
cd carspotter
```

### 2. Open the app

Just open the HTML file:

```bash
open car_spotter_final_3_5.html
```

No build step required.

---

## 🔐 Firebase Setup (Required for Sync)

Replace the Firebase config in the script with your own:

```js
firebase.initializeApp({
  apiKey: "...",
  authDomain: "...",
  projectId: "...",
});
```

Enable:

* Google Authentication
* Firestore Database

---

## ⚠️ Limitations

* Car values are user-entered (no external pricing API)
* No image support for cars
* Voice input depends on browser support (Chrome/Safari best)
* Single-file architecture (not modular)

---

## 💡 Future Improvements

* Car database integration (auto-fill values)
* Image uploads
* Social / leaderboard system
* GPS-based spotting
* Native mobile app version

---

## 🧩 Why This Exists

Car spotting is usually passive.

CarSpotter turns it into:

* A game
* A competition
* A personal collection system

---

## 📄 License

MIT License (or whatever you choose)

---

## 👤 Author

Built by a car enthusiast, for car enthusiasts.
