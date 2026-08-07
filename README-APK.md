# Android APK build setup

Place these files in the repository root alongside:

- `index.html`
- `styles.css`
- `app.js`
- `images/`
- `videos/`

The folder names must remain `images` and `videos` because the current app references those paths.

## Build

Push to the `main` branch or run **Build Android APK** manually from the GitHub Actions tab. Download `Form-Android-Debug-APK` from the completed run's Artifacts section.

## Notes

- This workflow produces a debug APK for testing and direct installation.
- Local images and GIFs do not need Android storage permissions.
- Cleartext traffic is disabled because the app uses packaged local assets. Only enable it if the app must load trusted `http://` resources.
- For Play Store distribution, add release signing and build an Android App Bundle (`.aab`) instead of using the debug APK.
