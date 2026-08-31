# Web To APK - In-App Purchases (IAP) Playground

This repository folder contains a focused, standalone boilerplate demonstrating Google Play In-App Purchases (IAP) integration via the `postMessage` bridge.

## 🚀 Features
- **Purchase Trigger (`order-iap`)**: Send purchase intent for consumable and non-consumable product IDs.
- **Restore Purchases (`restore-iap`)**: Request restoration of previously owned products/subscriptions.
- **Event Listener (`iap_approved`)**: Safely process incoming transaction payloads and purchase tokens.
- **Interactive Event Terminal**: Live diagnostic console for tracking bi-directional bridge events.

## 📚 Official Documentation
For exhaustive payload schemas, backend verification guidelines, and Android setup references:

**[👉 https://docs.dropcore.net/wta/](https://docs.dropcore.net/wta/)**

## 🛠️ Usage Flow

1. **Host Your Web App**: Deploy `iap/index.html` to a public web hosting service to obtain a live URL.
2. **Configure App Builder**:
   - Open the **Web To APK** app builder interface.
   - Enter your hosted live URL in the **WEBSITE URL** field.
   - Open **Plugins** (puzzle icon) and select **In-App Purchases**.
   - Configure your Google Play Billing product identifiers and save settings.
3. **Build APK**:
   - Select your output format (e.g., **Debug APK (Testing)** or **Release / AAB** for Google Play).
   - Tap **Build Application**.
4. **Test & Monitor**:
   - Install the build on a test device with a Google Play license testing account.
   - Trigger purchases from the UI and monitor incoming approval events inside the **Event Terminal**.