# EduSpace Android — Complete GitHub Actions Project

This ZIP contains the complete Android project. Upload the extracted contents to the root of a new or existing GitHub repository.

## Project contents
- `settings.gradle` — Gradle project settings
- `build.gradle` — Android Gradle Plugin configuration
- `gradle.properties` — Android/Gradle settings
- `app/build.gradle` — Android application configuration
- `app/src/main/AndroidManifest.xml` — Android app manifest
- `app/src/main/java/.../MainActivity.java` — Android WebView activity and file chooser
- `app/src/main/res/` — app theme and launcher vector
- `app/src/main/assets/www/` — complete educational app HTML, CSS, JS, PWA assets
- `.github/workflows/android-build.yml` — automatic APK build workflow

## Upload on mobile
1. Download this ZIP and extract it.
2. Open your GitHub repository in Chrome.
3. Use Add file → Upload files.
4. Select the extracted project files and folders, not the ZIP itself.
5. Make sure the `.github/workflows/android-build.yml` file is uploaded too. On Android file pickers, enable Show hidden files if needed, or upload `.github` contents through GitHub's create-file UI if the folder is hidden.
6. Commit the upload to `main`.

## Build
A push to `main` or `master` starts the workflow. You can also run it from Actions → Build EduSpace Android APK → Run workflow.

The APK is uploaded as the `EduSpace-debug-APK` artifact. Download the artifact ZIP and extract `app-debug.apk`.

## Important
- This is a debug APK for testing, not a signed Play Store release.
- The app is a native Android WebView shell containing the educational interface.
- Notes and files are stored locally on the device/browser profile. No cloud sync or login backend is included.
