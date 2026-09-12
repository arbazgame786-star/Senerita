# Senorita — build APK from a phone

This project includes a GitHub Actions workflow at `.github/workflows/build-apk.yml`.

1. Create a GitHub repository named `Senorita`.
2. Upload the project files/folder to the repository.
3. Open **Actions** → **Build Senorita APK** → **Run workflow**.
4. Wait for the green check.
5. Open the completed workflow run and download the **Senorita-debug-apk** artifact.
6. Extract the artifact ZIP and install `app-debug.apk` on the Android phone.

The workflow uses Java 17 and Gradle 9.6.0. It builds a debug APK, which is suitable for testing/installing on a phone. A Play Store release later needs a proper release signing key.
