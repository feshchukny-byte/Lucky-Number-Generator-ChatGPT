# Lucky Number Generator ChatGPT

Native Android app (Java). Choose any integer range from 0 to 100, inclusive. Press GENERATE to get a fresh SecureRandom result while the green number display spins and gradually slows. Tap HISTORY to view the last 10 results, saved on the device. No network access or permissions required.

## Build APK

1. Install Android Studio (JDK 17 and Android SDK 35).
2. Open this folder as an Android Studio project.
3. Let Gradle sync (requires internet on the development computer for first-time dependencies).
4. Choose **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
5. Install the APK located at `app/build/outputs/apk/debug/app-debug.apk`.

This download contains **source code, not a built APK**. Package name: `com.luckynumber.generator`.

## Build APK with GitHub Actions (without installing Android Studio)
1. Create a new GitHub repository and upload all files and folders from this project, including the hidden `.github/workflows/build-apk.yml` path.
2. Go to the **Actions** tab and choose **Build Android APK**.
3. Press **Run workflow** (or push the project to the default `main`/`master` branch).
4. When the workflow succeeds, download **LuckyNumberGeneratorChatGPT-debug-apk** from **Artifacts** in the workflow run. Unzip it to get `app-debug.apk`.
5. Transfer `app-debug.apk` to your Samsung and open it to install. Android may ask you to allow installs from that source.

This builds a *debug* APK. It is not a Play Store release, and the build has not been tested on a phone.
