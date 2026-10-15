# 3D Cube Lab — Android starter project

This is a starter Android WebView app with an interactive cube editor and classic painted-cube counting formulas.

## Important limits in this starter
- The 3D scene currently shows three faces in a CSS 3D view, not a full six-face 3D engine.
- The cut plane and separate-pieces mode are visual previews; they do not yet produce independently draggable solid pieces.
- Paint/erase acts on visible face tiles. Classic exam formulas are correct for a cube painted on all six outer faces and divided into equal n×n×n cubes.
- This source package does not itself contain a compiled APK. Use the cloud build steps below.

## Build an APK using only an Android phone
1. In your phone browser, sign in to GitHub and create a new repository.
2. Upload the contents of this folder to the repository (keep the folder structure).
3. Open the repository's **Actions** tab and enable Actions if prompted.
4. Select **Build Android APK** and tap **Run workflow**. Alternatively, pushing to `main` triggers a build.
5. Open the completed workflow run, find **Artifacts**, and download `3D-Cube-Lab-APK`.
6. Extract the downloaded ZIP and install `app-debug.apk`. Android may ask you to allow installation from your browser/files app.

## Technical
- Android app wrapper: Java + WebView
- UI and cube prototype: local `app/src/main/assets/index.html`
- Cloud build: GitHub Actions, JDK 17, Android SDK 35
- Internet is not required by the app at runtime; the prototype assets are local.
