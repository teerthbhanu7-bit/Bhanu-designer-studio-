# Bhanu Designer Studio — GitHub APK Builder

This is the Android/Capacitor project for **Bhanu Designer Studio** with a GitHub Actions workflow that automatically creates an installable Android **debug APK**.

## Fastest way to get the APK

1. Create a new GitHub repository, for example `bhanu-designer-studio-app`.
2. Upload **all files and folders inside this project** to the repository root.
3. Make sure the default branch is `main`.
4. Open **Actions** → **Build Android APK**.
5. Click **Run workflow**.
6. Wait for the workflow to finish.
7. Open the completed workflow run and download the artifact named:
   `bhanu-designer-studio-debug-apk`
8. Inside the downloaded ZIP is `app-debug.apk`. Install it on your Android phone.

The workflow also runs automatically whenever you push changes to `main`.

## What the workflow does

- Installs Node.js 20 and Java 21.
- Installs the Android SDK/platform tools.
- Installs the npm dependencies.
- Adds the Capacitor Android project.
- Builds the React/Vite web app.
- Syncs the web app into Android.
- Runs Gradle to build `app-debug.apk`.
- Uploads the APK as a GitHub Actions artifact.

## Important

This workflow produces a **debug APK** for testing/direct installation. It is not a Play Store release build. For Google Play, create a signed release build/AAB and keep the signing key in GitHub Actions secrets.

## App identity

- App name: Bhanu Designer Studio
- Package ID: `com.bhanudesignerstudio.app`
- Framework: React + Vite + Capacitor
