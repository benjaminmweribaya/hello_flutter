# 🧰 Flutter Beginner’s Toolkit

## 1. Title & Objective

**Title:** *Getting Started with Flutter – A Beginner’s Guide to Building Cross-Platform Apps*

* **Technology chosen:** Flutter (an open-source UI toolkit built by Google using the Dart language).
* **Why Flutter?**

  * Build apps for Android, iOS, Web, and Desktop from a single codebase.
  * Rapid development with **hot reload** and a rich widget ecosystem.
  * Strong community support and extensive documentation.
* **End goal:** Run a simple **“Hello, World!”** app on a connected Android device and document a clear setup process for beginners.

---

## 2. Quick Summary of the Technology

* **What is Flutter?**
  Flutter is a cross-platform framework that allows developers to build natively compiled applications using a widget-based architecture in the Dart language.

* **Where is it used?**

  * Mobile apps (Android and iOS)
  * Web applications
  * Desktop applications (Windows, Linux, macOS)

* **Real-world examples:**

  * Google Ads mobile app
  * BMW’s *My BMW* app
  * eBay Motors

---

## 3. System Requirements

* **Operating Systems supported:** Windows, macOS, or Linux
* **Hardware:**

  * \~10 GB free disk space
  * At least 8 GB RAM recommended
  * CPU virtualization enabled (if you plan to use emulators)
* **Tools & Editors:**

  * Flutter SDK
  * Android Studio or Visual Studio Code
  * Dart SDK (bundled with Flutter)
  * Android SDK & Platform-Tools
  * Git (for version control)

---

## 4. Installation & Setup Instructions

### Step 1: Install Flutter SDK

1. Download Flutter SDK for your OS: [Flutter Installation Guide](https://docs.flutter.dev/get-started/install).
2. Extract it (e.g., `C:\src\flutter` on Windows).
3. Add `flutter\bin` to your PATH environment variable.

### Step 2: Verify Installation

Open PowerShell and run:

```powershell
flutter doctor
```

This checks all dependencies (Android SDK, connected devices, editors).

### Step 3: Install Editor & Extensions

* **VS Code:** Install the Flutter and Dart extensions.
* **Android Studio:** Install Flutter and Dart plugins from *Settings → Plugins*.

### Step 4: Configure Android SDK

1. Open **Android Studio → SDK Manager** → install the latest **Android SDK Platform** and **Platform-Tools**.
2. Accept licenses in terminal:

   ```powershell
   flutter doctor --android-licenses
   ```
3. If using a real device: enable **Developer Mode** and **USB Debugging**.

---

## 5. Minimal Working Example

We’ll build a Flutter “Hello World” app.

### Step 1: Create a Project

```powershell
flutter create hello_flutter
cd hello_flutter
```

### Step 2: Replace `lib/main.dart` with:

```dart
import 'package:flutter/material.dart';

void main() => runApp(const MyApp());

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Hello World',
      theme: ThemeData(useMaterial3: true),
      home: const HomeScreen(),
    );
  }
}

class HomeScreen extends StatelessWidget {
  const HomeScreen({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(title: const Text('Flutter Hello World')),
      body: const Center(
        child: Text(
          'Hello, World! 👋',
          style: TextStyle(fontSize: 28, fontWeight: FontWeight.w600),
        ),
      ),
    );
  }
}
```

### Step 3: Run on device

```powershell
flutter run
```

**Expected Output:**

* App bar with title: *Flutter Hello World*
* Centered text: *Hello, World! 👋*

---

## 6. AI Prompt Journal

| Prompt Used                                                                             | AI’s Response (Summary)                                                                                                                      | Reflection                                                 |
| --------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| “Give me a step-by-step guide to install Flutter on Windows and run a Hello World app.” | Listed SDK download, PATH setup, Android Studio install, project creation.                                                                   | Helped me scaffold the environment correctly.              |
| “`flutter doctor` says ‘Android SDK not found’. Show me how to fix this.”               | Guided me to install SDK via Android Studio and accept licenses.                                                                             | Solved setup blockers quickly.                             |
| “Create a minimal Flutter `main.dart` that shows Hello World with Material 3.”          | Gave a widget tree with MaterialApp, Scaffold, Text widget.                                                                                  | Clear code, helped me understand widget hierarchy.         |
| “How do I run a Flutter app on a physical Android device via USB?”                      | Explained enabling Developer Mode, turning on USB Debugging, accepting device authorization, then using `flutter devices` and `flutter run`. | Helped me successfully test on real hardware.              |
| “Gradle task assembleDebug failed – how can I fix it?”                                  | Suggested deleting Gradle cache, running `flutter clean`, then `flutter pub get`.                                                            | Resolved my Gradle build errors and unblocked the project. |

---

## 7. Common Issues & Fixes

* **Issue:** `flutter doctor` → Android SDK not found.

  * *Fix:* Install SDK in Android Studio and run `flutter doctor --android-licenses`.

* **Issue:** No devices detected.

  * *Fix:* Enable USB Debugging on device or create an emulator in AVD Manager.

* **Issue:** Emulator not starting.

  * *Fix:* Enable virtualization in BIOS, cold boot AVD, or use physical device.

* **Issue:** `Gradle task assembleDebug failed`.

  * *Fix:* Run `flutter clean`, delete `.gradle` cache, then `flutter pub get`.

---

## 8. References

* [Flutter Official Docs](https://docs.flutter.dev/)
* [Dart Language Docs](https://dart.dev/guides)
* [Flutter YouTube Channel](https://www.youtube.com/c/flutterdev)
* [StackOverflow: Flutter Issues](https://stackoverflow.com/questions/tagged/flutter)

---