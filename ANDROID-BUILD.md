# Bhanu Designer Studio — Android APK Build Project

This is a Capacitor Android wrapper around the React/Vite app.

## Requirements
- Node.js 20+
- Android Studio (latest stable)
- Android SDK + platform tools
- JDK 17

## First setup
```bash
npm install
npx cap add android
```

## Build web app and sync Android
```bash
npm run build:android
```

## Open Android Studio
```bash
npx cap open android
```

Then in Android Studio use **Build → Build Bundle(s) / APK(s) → Build APK(s)**.

The debug APK will normally be under:
`android/app/build/outputs/apk/debug/app-debug.apk`

For a Play Store release, create a signed release build in Android Studio and configure your signing key.

## App identity
- App name: Bhanu Designer Studio
- Package ID: `com.bhanudesignerstudio.app`
- Theme colors: ivory / maroon / royal gold

## AI Try-On
The UI currently calls the frontend demo flow. Connect the production `/api/try-on` endpoint to a real virtual try-on provider before release. Keep provider API keys on a server; never put them in the Android app.
