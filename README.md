# Pitch Ready — Android wrapper

The Pitch Ready standalone demo (`app/src/main/assets/index.html`) in a WebView.

* No permissions, no network — the whole app is one offline HTML file.
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
