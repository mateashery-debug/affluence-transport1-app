# Affluence Transport Services Android app

## Included
- Customer-facing home screen and service list
- Transport request form
- Local/offline storage of requests on the device
- Business dashboard to view, share, and delete saved requests
- Tap-to-call contact numbers
- WhatsApp enquiry and booking hand-off
- Murewa base / nationwide delivery message

## Build an APK
1. Install Android Studio (latest stable) on a computer.
2. Open this project folder in Android Studio.
3. Allow Gradle sync and install any requested Android SDK platform (API 35).
4. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. Android Studio will show the generated APK location, usually `app/build/outputs/apk/debug/app-debug.apk`.
6. Copy the APK to your Android phone and install it. You may need to allow installation from that file manager.

## Important limitations in this starter version
- Bookings are stored locally on the phone that created them. There is no shared cloud database or live multi-phone synchronization yet.
- Submitting a booking opens WhatsApp with a prefilled message to the business number. The customer must tap Send.
- The Manage screen is not password-protected yet. Add authentication before giving the app to customers or publishing it.
- Update the WhatsApp destination number if a different business WhatsApp line should receive bookings.
- This project is a starter source project, not a prebuilt APK.

## Build the APK online using only an Android phone (GitHub Actions)
This project includes `.github/workflows/android.yml` for a cloud build.
1. Sign in to GitHub in your phone browser and create a new repository (for example `AffluenceTransport`).
2. Upload the contents of this ZIP into the repository, keeping the folder structure. The files inside `AffluenceTransportApp` should be at the repository root (including the `.github` folder).
3. Open the repository's **Actions** tab and select **Build Android APK**. If prompted, enable Actions, then choose **Run workflow**.
4. Wait for the workflow to finish successfully. Open the completed run and download the **Affluence-Transport-APK** artifact.
5. Extract the downloaded artifact ZIP on your phone, tap `app-debug.apk`, and follow Android's installation prompts. Allow installs from your browser or file manager if Android asks.

The APK is a debug-signed installable build for testing, not a Play Store release. The dashboard and saved bookings are local to one device in this version.
