# EduSpace Android App — GitHub Actions Build

This repository is an Android APK project. The educational dashboard is bundled inside a native Android WebView shell.

## Build APK with GitHub Actions

1. Create a new GitHub repository.
2. Extract this ZIP and upload **all contents** to the repository root. Keep the `.github/workflows/android-build.yml` path intact.
3. Commit the files to the `main` branch.
4. Open the repository's **Actions** tab.
5. Select **Build EduSpace Android APK** and open the latest successful run.
6. Under **Artifacts**, download `EduSpace-debug-APK`. Extract it to get `app-debug.apk`.
7. Transfer the APK to your Android phone and install it. Android may ask you to allow installation from that source.

## Automatic builds

- Every push to `main` or `master` automatically starts an APK build.
- You can also run it manually from **Actions → Build EduSpace Android APK → Run workflow**.
- No GitHub Pages deployment or separate website build is required for the APK.

## App features in this starter

- Student dashboard and course cards
- Add course subjects
- File library: stores selected files locally using browser IndexedDB
- Personal notes using local browser storage
- Basic Electrical sample MCQ quiz
- Light/dark theme
- Responsive app-style layout

## Important notes

- This workflow creates a **debug APK** for testing, not a Play Store release.
- Uploaded resources and notes remain on that device/app installation. There is no cloud account or cross-device sync yet.
- The Android app is a native Android wrapper around the bundled HTML/CSS/JS learning interface. Native features, notifications, authentication, cloud sync and Play Store signing can be added in later versions.
- Package ID: `com.lkstudystudio.eduspace`
- Version: `1.0`
