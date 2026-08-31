# Web To APK - API Playground

Welcome to the Web To APK API Playground repository. This project serves as a practical demonstration and boilerplate for integrating native Android features into your web application using the `postMessage` bridge.

## 🚀 Features
- **Google AdMob API**: Controls and event listeners for Banner, Interstitial, and Rewarded Video Ads.
- **Interactive Event Terminal**: Real-time logging of native bridge communication.

## 📚 Official Documentation
For complete guides, configuration parameters, and exact action references:

**[👉 https://docs.dropcore.net/wta/](https://docs.dropcore.net/wta/)**

## 🛠️ Usage Flow

1. **Host Your Web App**: Deploy `index.html` to a public web hosting service (e.g., GitLab Pages, Vercel, Netlify) to obtain a live URL.
2. **Configure App Builder**:
   - Open the **Web To APK** app builder interface.
   - Enter your hosted live URL in the **WEBSITE URL** field.
   - Open **Plugins** (puzzle icon) and select **Google AdMob**.
   - Input your AdMob Ad Unit IDs (or official Test Ad Unit IDs) and click **Save AdMob**.
3. **Build APK**:
   - Select your output format (e.g., **Debug APK (Testing)**).
   - Tap **Build Application** to generate the Android package.
4. **Test & Monitor**:
   - Install and launch the APK on an Android device.
   - Interact with the ad triggers on screen and inspect the live logs inside the built-in **Event Terminal**.