RAYAN'S LIFE RPG — SHADOW SYSTEM V2.0
=====================================

WHAT IS INCLUDED
- Offline-first dark fantasy RPG dashboard.
- Local XP, levels, coins, daily missions and streak tracking.
- Skills, achievements, MMA training log, drawing practice journal and hygiene mission.
- Focus Academy with three offline mini-games:
  * Memory Trial
  * Number Sequence
  * Pattern Focus
- Each focus mini-game awards +10 XP and +5 coins once per local device day.
- Five Demon Warrior evolution stages based on player level:
  * Stage I — Shadow Rookie (Level 1)
  * Stage II — Shadow Knight (Level 5)
  * Stage III — Dark Warrior (Level 10)
  * Stage IV — Shadow Lord (Level 25)
  * Stage V — Demon King (Level 50)
- Animated evolution scene using CSS 3D-style layered artwork. This is not a true 3D mesh/model.
- Local PIN, sound effects, synthesized ambient audio, themes and background image.
- Local JSON backup export/import.
- Service worker for offline caching.
- Capacitor configuration and GitHub Actions workflow for Android debug APK builds.

IMPORTANT LIMITATIONS
- Focus games are locally generated and work offline; they are not live AI-generated challenges.
- The evolution cinematic is a CSS 3D-style scene, not a true real-time 3D model or 3D character rig.
- Automatic AI drawing critique, cloud sync and online multiplayer are not included.
- Drawing feedback remains a practice journal/checklist. AI image critique requires a separately configured online or on-device AI service and explicit image permission.
- Progress is stored in this browser/device. Export a backup before clearing browser data or reinstalling.

QUICK TEST ON ANDROID
1. Upload the project files to a GitHub repository (upload the extracted files, not only this ZIP).
2. Enable GitHub Pages: Settings > Pages > Deploy from a branch > main > /(root) > Save.
3. Open the published HTTPS site once while online.
4. In Chrome, use menu > Add to Home screen / Install app.
5. Open the installed app once online so its files can be cached for offline use.

BUILD A NATIVE APK WITH GITHUB ACTIONS
1. Upload all extracted project files, including the .github folder, to the repository.
2. Open the Actions tab.
3. Choose "Build Android APK" and select Run workflow (or push a commit to main).
4. Wait for the workflow to finish successfully.
5. Open the completed workflow run and download the rayans-life-rpg-debug-apk artifact.
6. Extract the downloaded artifact ZIP and install app-debug.apk on your Android phone.

LOCAL APK BUILD (requires a computer)
1. Install Node.js LTS and Android Studio with Android SDK.
2. Extract this project.
3. Run npm install.
4. Run npx cap add android (only if the android folder does not exist).
5. Run npx cap sync android.
6. Run npx cap open android.
7. In Android Studio, build the debug APK.

SECURITY / PRIVACY
- The PIN is a convenience lock, not a secure account system. Clearing app data or reinstalling may reset it.
- Android does not allow a normal app to disable the Home button or trap the user inside the app.
- Audio begins only after a user gesture, as required by browser policies.
- No account or cloud sync is included. Keep regular local backups.
