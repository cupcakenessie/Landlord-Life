# LANDLORD LIFE — Phone-only Android publishing route

You can prepare the release from an Android phone without installing Unity.

## 1. Create a GitHub repository
Create a new repository named `landlord-life` and upload this folder's contents from your phone.

## 2. Run the build
Open **Actions → Build LANDLORD LIFE Android AAB → Run workflow**.
GitHub will build the Android App Bundle using Android SDK 36 and save the `.aab` as an artifact.

For the first build, the workflow creates a temporary upload keystore and stores it with the artifact. Download and keep that keystore private. For future releases, configure GitHub repository secrets so the same upload key is used.

## 3. Google Play Console
Create the app as a **Game**, free initially, and use the package name `com.landlordlife.game`. Package names are permanent once registered, so do not change it after creating the Play app.

Official Play Console: https://play.google.com/console/

## 4. Upload the AAB
Use **Testing → Internal testing** first. Upload the AAB artifact from GitHub Actions.

## 5. Closed testing
If your Play Console account is a new personal account, Google currently requires at least 12 testers opted into the closed test continuously for 14 days before production access can be requested.

## 6. Production
After the closed-test requirement and Play Console app setup are complete, apply for production access, answer the testing/production questions, then create a Production release with the tested AAB.

## Important
This package contains the game and the build pipeline. It does not create a Google Play developer account, perform identity verification, pay registration fees, or publish on your behalf. Those steps require your Google account and your approval.


## Android release target
Minimum supported Android version: Android 13 (API 33). Target/compile SDK: Android 16 (API 36).
