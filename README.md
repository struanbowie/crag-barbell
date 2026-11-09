# Crag & Barbell

A personal full-body gym plan for climbers, packaged as an offline Android app.

The whole app is one page: `app/src/main/assets/index.html`. Edit that file and push to `main`;
GitHub Actions builds a signed APK and publishes it as a new release.

## Install on Android

1. Install [Obtainium](https://github.com/ImranR98/Obtainium) (from F-Droid or its GitHub releases).
2. In Obtainium, tap **Add app** and paste this repository's URL.
3. Tap **Install**. Obtainium checks for new releases and offers updates.

## Build secrets

The workflow signs every build with the same key so updates install over the old version.
It needs these repository secrets: `KEYSTORE_BASE64`, `KEYSTORE_PASSWORD`, `KEY_ALIAS`.
