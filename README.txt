RAYAN'S LIFE RPG — ANDROID STARTER PROJECT
===========================================

WHAT IS INCLUDED
- Offline-first web app dashboard with a dark fantasy theme.
- Local XP, levels, coins, daily missions and streak tracking.
- Skills, achievements, MMA training log, drawing practice journal.
- Name/theme/background customization.
- Local JSON backup export/import.
- Service worker for offline caching.
- Capacitor configuration for building an Android app.

IMPORTANT LIMITATIONS
This is a working starter app, not a signed APK. It does not include a 3D animated warrior,
automatic AI drawing critique, cloud sync, or mini-games yet. Drawing feedback is a practice
journal/checklist in this offline edition. AI image critique requires an on-device model or
an internet-connected service and explicit image permission.

QUICK TEST ON ANDROID
1. Extract this ZIP.
2. Host the folder on HTTPS (or run it locally through a development server).
3. Open index.html from a local web server in Chrome. Service workers generally do not work
   when opening a file:// URL directly.
4. In Chrome, use menu > Add to Home screen / Install app.
   For offline use, open it once while online so its files are cached.

BUILD A NATIVE APK (requires a computer)
1. Install Node.js LTS and Android Studio with Android SDK.
2. Extract this project.
3. In a terminal, run:
     npm install
     mkdir www
     copy index.html, manifest.webmanifest and sw.js into www/
   On macOS/Linux use: mkdir -p www && cp index.html manifest.webmanifest sw.js www/
4. Run:
     npx cap add android
     npx cap sync android
     npx cap open android
5. In Android Studio, wait for Gradle sync. Choose Build > Build Bundle(s) / APK(s) > Build APK(s).
6. Test the generated APK on your own Android phone before sharing it.

NOTE: For native photo/camera pickers, app signing, Play Store release, and production-grade
offline image storage, additional Android integration and testing are required.


SHADOW SYSTEM UPGRADE (v1.1)
- 5-second animated intro and Enter gate.
- Local PIN setup / unlock and PIN change.
- Synthesized local SFX and ambient background soundtrack controls.
- Evolving SVG shadow demon companion and level-up animation.
- Glassmorphism panels and fantasy handwritten-style headings.

SECURITY / ANDROID NOTES
- The PIN is a convenience lock stored on this device. It is not a secure account system;
  clearing app data or reinstalling can reset it. Keep your device lock enabled.
- Android does not permit an ordinary app to disable the system Home button or trap a user
  inside the app. True kiosk/lock-task mode requires Android device-owner or managed-device
  setup and should only be used with an authorized administrator.
- Audio starts only after the user taps its control because Android requires a user gesture.
- The demon artwork is an original inline vector with CSS animation; it is not a 3D model.
- For a native APK, use the Capacitor steps above. Install Android Studio/SDK and Node.js free.
- Sideloading a debug/release APK to your own phone can be free. Google Play publishing
  generally requires a one-time Play Console registration fee (currently US$25, subject to
  Google's current rules and regional taxes).
