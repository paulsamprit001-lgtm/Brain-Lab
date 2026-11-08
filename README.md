# Brain Lab for Android

This repository packages the original Brain Lab HTML app as an Android app using Capacitor.

## Build an APK

1. Open the **Actions** tab in this GitHub repository.
2. Select **Build Brain Lab APK**.
3. Press **Run workflow** (or wait for a build after a push to `main`).
4. Open the completed workflow run and download the **Brain-Lab-debug-APK** artifact.
5. Extract the downloaded ZIP to get `app-debug.apk`.

The APK is a debug build for testing and direct installation. It is not a Play Store release.

## App data

Game progress is stored locally on the device using browser storage inside the Android WebView. The original HTML also contains JSON backup and restore controls.

The original HTML optionally checks for a Claude-hosted `window.claude` database/user bridge. A standard Android WebView does not provide that bridge, so account-based cloud sync is not active in this APK; local progress and in-app backup/restore remain available.

## Project details

- App name: Brain Lab
- Android application ID: `com.brainlab.app`
- Web app source: `www/index.html`
- Android wrapper: Capacitor 7
