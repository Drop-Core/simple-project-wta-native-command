# Web To APK Builder - Native API Example Projects

This repository contains simple, ready-to-use HTML5 project templates demonstrating how to integrate native device features (AdMob, In-App Purchases, Camera, Geolocation, etc.) using the **Web To APK Builder**.

## 🚀 Quick Testing Guide

You can quickly test these example projects directly in the App Builder without writing any code.

1. **Download the Repository:** Click the green **`<> Code`** button at the top of this page and select **`Download ZIP`**.
2. **Extract:** Extract the downloaded `simple-project-wta-native-command-main.zip` file to your computer.
3. **Select a Module:** Open the extracted folder and pick one specific feature you want to test (for example, the `admob` folder).
4. **Compress:** Right-click the chosen folder (e.g., `admob`) and compress/zip it. You will get a file named `admob.zip`.
5. **Build:** Open the Web To APK Builder, select the **Offline .ZIP** tab, upload your `admob.zip`, and click **Build Application**.

---

## 📦 Offline .ZIP Upload Guide

To ensure your app compiles successfully without showing a blank white screen, you **must** follow this strict folder structure and compression method.

### 1. Mandatory Folder Structure
The main `index.html` file must be located exactly at the root of your project folder. It cannot be hidden inside a sub-folder.

✅ **CORRECT STRUCTURE:**
```text
my-awesome-game/
├── index.html       <-- MUST be here
├── css/
│   └── style.css
├── js/
│   └── game.js
└── assets/
    └── logo.png
```

❌ **INCORRECT STRUCTURE (Will result in a blank app):**
```text
my-awesome-game/
└── www/             <-- EXTRA FOLDER
    ├── index.html   <-- WRONG LOCATION
    ├── css/
    └── js/
```

### 2. Compression (Zipping) Rules
**Do not ZIP the files inside the folder directly. You must ZIP the main project folder itself.**

*   **How to do it correctly:** Right-click on the `my-awesome-game` folder -> Select **Compress/Zip**. The result will be `my-awesome-game.zip`.
*   **Why?** This ensures our system extracts your project into a single, clean container without overlapping with the builder's internal core system.

---

## 🔗 URL Link Guide (Live Hosted Web Apps)

If you prefer to build an app from a live website instead of an offline `.zip` file, follow these steps:

1. **Host Your Web App:** Deploy your `index.html` and assets to a public web hosting service (e.g., GitHub Pages, Vercel, Netlify, or a VPS) to obtain a live URL.
2. **Configure App Builder:** Open the Web To APK app builder interface and set up your App Name and Package ID.
3. **Enter URL:** Select the **URL Link** tab and enter your hosted live URL in the `WEBSITE URL` field (e.g., `https://my-awesome-app.vercel.app`).
4. **Configure Plugins:** Open the Plugins menu (the puzzle icon). If you want to monetize, select **Google AdMob**, enable it, input your AdMob Ad Unit IDs (or check the Test Mode switch), and click **Save AdMob**.
5. **Build APK/AAB:** Select your desired output format (e.g., `Debug APK (Testing)` for quick tests or `Release AAB` for Play Store submission).
6. **Generate:** Tap **Build Application** to generate your native Android package.