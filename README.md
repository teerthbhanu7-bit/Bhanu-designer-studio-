# Bhanu Designer Studio — Ready-to-Build Android App

This repository builds an installable Android APK automatically with GitHub Actions.

## Get the APK (no Android Studio required)

1. Create a new **empty** GitHub repository named `bhanu-designer-studio-app`.
2. Upload **all files in this folder** to the repository root.
3. Push to the `main` branch.
4. Open **Actions** → **Build Android APK**.
5. Open the completed run and download **bhanu-designer-studio-debug-apk**.
6. Extract the downloaded ZIP and install `app-debug.apk` on your Android phone.

You can also run it manually from **Actions → Build Android APK → Run workflow**.

## Automatic rebuilds

Every push to `main` automatically creates a fresh APK artifact.

## App details

- App name: **Bhanu Designer Studio**
- Package ID: `com.bhanudesignerstudio.app`
- React + Vite + Capacitor 7
- Debug APK for direct Android installation

## Important

The generated APK is a debug/test build. For Google Play Store publishing, a signed release AAB/APK and a secure signing key are required.
