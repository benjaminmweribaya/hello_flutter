# 📱 hello\_flutter

A beginner-friendly Flutter project showcasing a minimal **“Hello, World!”** app.
This project was created as part of the **Moringa School – AI Launchpad Capstone Project**, demonstrating how generative AI can accelerate learning and development in new technologies.

---

## 👤 Author

**Name:** Benjamin Mweri Baya
**Role:** Full-Stack Software Engineer 
**Project:** AI Launchpad Capstone – Beginner’s Toolkit with Flutter

---

## 🎯 Objective

The goal of this project is to:

* Learn Flutter using AI-powered prompts.
* Build and run a **minimal working example app**.
* Document setup instructions so anyone can reproduce the process.
* Share lessons learned, common issues, and troubleshooting strategies.

---

## 📝 Prerequisites

Before running this project, make sure you have:

* ✅ [Flutter SDK](https://docs.flutter.dev/get-started/install) installed and added to your PATH
* ✅ [Android Studio](https://developer.android.com/studio) or [Visual Studio Code](https://code.visualstudio.com/) with Flutter & Dart extensions
* ✅ Android SDK & Platform-Tools installed (via Android Studio SDK Manager)
* ✅ Either:

  * An **Android emulator** (AVD Manager)
  * OR a **physical Android device** with **USB debugging enabled**

---

## ⚡ Quick Start

```powershell
# 1) Create the project (if not already created)
flutter create hello_flutter
cd hello_flutter

# 2) Replace the generated lib/main.dart with the version in this repo

# 3) Fetch dependencies
flutter pub get

# 4) Run the app on an emulator or connected device
flutter run
```

---

## 👀 Expected Output

When you run the app, you should see:

* An **AppBar** titled *Flutter Hello World*
* A **centered text** message:

```
Hello, World! 👋
```

---

## 🧩 Project Structure

```
hello_flutter/
│ pubspec.yaml # Project metadata & dependencies
│ README.md # Project documentation
│
├───.dart_tool/ # Dart/Flutter internal tooling files
├───.idea/ # IntelliJ/Android Studio project settings
├───android/ # Android-specific code (Gradle, Kotlin, resources)
├───build/ # Build output (generated, can be cleaned)
├───docs/ # Project documentation (toolkit, journals, etc.)
├───ios/ # iOS-specific code (Xcode project, Swift, assets)
├───lib/ # Main application source code
│ └───main.dart # Entry point of the Flutter Hello World app
├───linux/ # Linux desktop build support
├───macos/ # macOS desktop build support
├───test/ # Example widget tests
├───web/ # Web app build support (HTML, manifest, icons)
├───windows/ # Windows desktop build support
└───.metadata # Flutter project metadata (auto-generated)
```

---

## 🛠️ Troubleshooting

* **Run environment checks:**

  ```powershell
  flutter doctor
  ```

  Resolve any issues shown.

* **Accept Android licenses:**

  ```powershell
  flutter doctor --android-licenses
  ```

* **If build fails:**

  ```powershell
  flutter clean
  flutter pub get
  flutter run
  ```

* **Device not detected?**

  * Ensure **USB Debugging** is enabled on your phone.
  * Run `flutter devices` to confirm detection.
  * For emulators: make sure virtualization is enabled in BIOS and AVD is launched from Android Studio.

---

## 📚 Learning with AI

This project was scaffolded with the help of **AI prompts**, which guided:

* Flutter SDK installation & PATH setup
* Android Studio configuration
* Project creation with `flutter create`
* Writing a minimal `main.dart` with Material 3 theme
* Debugging common Gradle/SDK issues

*(See `docs/Flutter_Beginners_Toolkit.md` for detailed documentation and AI prompts used.)*

---

## 🔗 References

* [Flutter Official Docs](https://docs.flutter.dev/)
* [Dart Language Guide](https://dart.dev/guides)
* [Flutter YouTube Channel](https://www.youtube.com/c/flutterdev)
* [StackOverflow – Flutter Tag](https://stackoverflow.com/questions/tagged/flutter)

---

## 📜 License

This project is released under the **MIT License**.
See [LICENSE](./LICENSE) for details.

---


