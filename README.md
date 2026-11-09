# BINUS Campus Map
An Android application that lets users browse four BINUS campus locations and view each one on Google Maps.

## Features

- Browse BINUS @AlamSutera, @Anggrek, @Bandung, and @Bekasi in a two-column campus list.
- Open a campus map with a marker and a close-up camera view of its fixed coordinates.

## Screenshots

### Campus List
![Campus list screen](https://github.com/temptedwithouta/google_map_api_android/assets/93007514/38f6f329-b490-488e-8308-5af32afade88)

### Campus Maps
- BINUS @AlamSutera
![Screenshot_20231201_162213_Gslc_2](https://github.com/temptedwithouta/google_map_api_android/assets/93007514/d4ff95c9-1780-4c69-8342-97a6e5a7dcf0)

- BINUS @Anggrek
![Screenshot_20231201_162353_Gslc_2](https://github.com/temptedwithouta/google_map_api_android/assets/93007514/dbc0d2f6-6713-407a-b3e0-cdc113be4595)

- BINUS @Bandung
![Screenshot_20231201_162248_Gslc_2](https://github.com/temptedwithouta/google_map_api_android/assets/93007514/ee685c59-5108-4927-85b0-dceccedc6eda)

- BINUS @Bekasi
![Screenshot_20231201_162314_Gslc_2](https://github.com/temptedwithouta/google_map_api_android/assets/93007514/92f789c2-fb7a-419a-bc55-014c0bb27838)

## Technology

- Java
- Android SDK: compile/target API 34, minimum API 24
- Google Maps SDK for Android 18.1.0
- AndroidX AppCompat, Material Components, and ConstraintLayout
- Gradle 8.2 with Android Gradle Plugin 8.2.0

## Requirements

- Android Studio with Android SDK 34 installed
- JDK 17 for the Android Gradle Plugin
- Android device or emulator running Android 7.0 (API 24) or later
- Google Play services and internet access for Google Maps
- A Google Maps API key with Maps SDK for Android enabled

## Setup and Run

1. Clone this repository and open it in Android Studio.
2. Create a Google Maps API key and enable the Maps SDK for Android in Google Cloud Console.
3. Restrict the key to the Android app (`com.example.gslc_2`) and the appropriate signing certificate. A key is currently embedded in `app/src/main/AndroidManifest.xml`; replace it with your own restricted key and rotate the exposed key before distributing the app. Do not commit API keys to version control.
4. Sync the project with Gradle, then run the `app` configuration on a device or emulator.

To build a debug APK from the command line:

```powershell
.\gradlew.bat assembleDebug
```

On macOS or Linux:

```bash
./gradlew assembleDebug
```

## Project Structure

```text
app/
	src/main/java/com/example/gslc_2/  # Activities, campus model, and list adapter
	src/main/res/                      # Layouts, images, and app resources
	src/test/                          # Local unit tests
	src/androidTest/                   # Instrumented Android tests

```

## License

No license is currently specified in this repository.
