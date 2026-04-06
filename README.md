# ShildX – Android Project Setup Guide

Welcome to **ShildX**! This guide will help you set up and run the project smoothly on your local machine using **Android Studio**.

---

## Prerequisites

Before you begin, ensure you have the following installed:

* **Android Studio** (Latest version recommended)
* **Java JDK 11 or higher**
* Android SDK (installed via Android Studio)
* Internet connection (for dependencies)

### Optional (Based on Project Type)

* **Node.js + npm** (for React Native projects)
* **Flutter SDK** (for Flutter projects)

---

## Project Setup

### Clone or Download the Repository

```bash
git clone https://github.com/your-username/ShildX.git

cd ShildX
```

OR download ZIP and extract it.

---

### Open Project in Android Studio

1. Open **Android Studio**
2. Click **Open**
3. Select the `ShildX` project folder
4. Click **OK**

---

### Sync Gradle

* Android Studio will automatically start syncing.
* If not:

  ```
  File → Sync Project with Gradle Files
  ```

---

## Running the Project

### Run on Emulator

1. Go to:

   ```
   Tools → Device Manager
   ```
2. Click **Create Device**
3. Select a device (Pixel recommended)
4. Choose Android version (API 33+)
5. Start emulator

---

### Run the App

* Click the **Run button** in Android Studio
* Select your device
* Wait for build & installation

---

## Project Type Detection

### Native Android (Java/Kotlin)

Look for:

```
app/src/main/java/
```

No extra setup needed

---

### React Native Project

Look for:

```
package.json
```

#### Run these commands:

```bash
npm install
npx react-native start
```

Then run Android app from Android Studio.

---

### Flutter Project

Look for:

```
pubspec.yaml
```

#### Run:

```bash
flutter pub get
flutter run
```

---

## ❌ Troubleshooting

### Gradle Build Failed

```
File → Invalidate Caches & Restart
```

---

### SDK Not Found

```
File → Project Structure → SDK Location
```

Set correct SDK path.

---

### License Issues

```bash
sdkmanager --licenses
```

---

### Emulator Not Working

* Enable **Virtualization (VT-x / AMD-V)** in BIOS

---

## Project Structure (Typical)

```
ShildX/
├── app/
├── gradle/
├── build.gradle
├── settings.gradle
└── ...
```

---
## License

This project is licensed under the MIT License.

---

## Need Help?

If you face any issues:

* Open an issue on GitHub
* Or contact the project maintainer

---
