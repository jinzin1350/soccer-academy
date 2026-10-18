# Pitch Ready — Android wrapper

The Pitch Ready standalone demo (`app/src/main/assets/index.html`) in a WebView.

* One HTML file in a WebView, talking to a Supabase backend over HTTPS.
* Internet is the only permission.
* Coach and parent share one academy through a six-letter code each.
* `minSdk 26` (Android 8.0), portrait, adaptive launcher icon.
* The release build is debug-signed so the APK sideloads without a keystore.

## Getting the APK

Every push to `main` builds it. Grab it from the latest
[release](../../releases) or from the run's artifacts under **Actions**.

## Updating the app

Replace `app/src/main/assets/index.html` and push. That is the only file that
carries the product.

## Building locally

    ./gradlew assembleRelease     # app/build/outputs/apk/release/
