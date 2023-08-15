# How to Create a Release

When releasing, we use a <strong>manual release</strong> system to ensure that both versions of the app go the the store at the same time and associations can be notified ahead of time. By following the steps listed below, you should be able to successfully release a new version of the app.

## Google Play Store
1) Update the version number in the pubspec.yaml file. (Increase the #.#.# and the number after the +)
2) In your IDE, run the command "flutter build appbundle"
3) Remember where the build was saved (Usually build\app\outputs\bundle\release\app-release.aab)
4) Login to the Google Play Console (https://play.google.com/console)
5) Go to the Production page under the Release header and click "Create new release"
6) Add the app bundle, finish the following steps to save the changes.
7) On the Publishing Overview page, send the change for review (This will not release the app)
8) When ready to launch to store, manually launch.

## Apple App Store
1) Update the version number on the target Runner
2) Create an archive (Product -> Archive)
4) Select the Archive and click Distribute App
5) Select Okay for most popups.
6) Log in to App Store Connect (https://appstoreconnect.apple.com)
7) Go to the TestFlight page for the app and wait for the archive to finish uploading
8) Press the warning and select "No Encryption"
9) On the app store page, create a new version, add the build and an update description
10) Submit the version for review
11) When ready to launch to store, select release

