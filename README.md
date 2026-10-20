# Rabat Astrolabe — Wear OS app (WebView wrapper)

Offline astrolabe/watch face (assets/index.html) wrapped in a Wear OS app.

## Build the APK
A) GitHub (no installs): create a new GitHub repo, upload this folder's contents, open
   Actions > "Build APK" > Run workflow, then download the artifact `app-debug.apk`.
B) Android Studio: File > Open this folder, wait for sync, Build > Build APK(s).

## Install on a Pixel Watch (LTE)
1. Watch: Settings > System > About > Versions > tap "Build number" 7 times.
2. Settings > Developer options > turn on ADB debugging and Wireless debugging.
3. Wireless debugging > Pair new device (note IP:port and code).
4. PC: `adb pair IP:PORT` (enter the code), then `adb connect IP:PORT2`.
5. `adb install app-debug.apk` -> open "Rabat Astrolabe" in the app list.
