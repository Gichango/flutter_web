# Getting Started with Flutter Web Using Dart – A Beginner’s Guide

## 1. Title & Objective
**Title:** Getting Started with Flutter Web Using Dart – A Beginner’s Guide

**Objective:**
This toolkit introduces beginners to **Flutter Web**, a feature of the Flutter framework that enables developers to build cross-platform applications (mobile, web, desktop) using the Dart programming language. By the end of this guide, you’ll be able to set up Flutter Web on your system and run a minimal “Hello World” webpage.

---

## 2. Quick Summary of the Technology
- **Dart** is a programming language developed by Google, optimized for UI and cross-platform development.
- **Flutter** is a UI framework for building apps for mobile, web, and desktop from a single codebase.
- **Flutter Web** allows you to compile Flutter applications into standards-based web apps that run in modern browsers.

---

## 3. System Requirements
- **Operating System:** Windows / macOS / Linux
- **Tools & Editors:** Flutter SDK (includes Dart), VS Code or Android Studio, Chrome browser
- **Packages:** None required (Flutter Web support is built in)

---

## 4. Installation & Setup Instructions
1. Install Flutter SDK: https://docs.flutter.dev/get-started/install
2. Add Flutter to PATH (add flutter/bin)
3. Verify installation:
   ```bash
   flutter doctor
   ```
4. Enable web support:
   ```bash
   flutter config --enable-web
   flutter devices
   ```
5. Create & run a project:
   ```bash
   flutter create hello_flutter_web
   cd hello_flutter_web
   flutter run -d chrome
   ```

---

## 5. Minimal Working Example (lib/main.dart)
Paste the following into `lib/main.dart` and run the app:

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Web Demo',
      home: Scaffold(
        appBar: AppBar(
          title: const Text('Flutter Web Hello World'),
        ),
        body: const Center(
          child: Text(
            'Hello, Flutter Web!',
            style: TextStyle(fontSize: 24),
          ),
        ),
      ),
    );
  }
}
```

**Expected Output:** A Chrome window opens showing an AppBar titled *Flutter Web Hello World* and centered text *Hello, Flutter Web!*

---

## 6. AI Prompt Journal
Example prompts used during development:
- "How do I enable Flutter Web on my system?" → Guided to `flutter config --enable-web`.
- "Give me a simple Hello World example for Flutter Web." → Provided the base code used above.
- "How do I fix 'No web devices found'?" → Solution: enable web and check Chrome installation.

---

## 7. Common Issues & Fixes
- **No web devices found** → Run `flutter config --enable-web`.
- **Chrome not detected** → Ensure Chrome is installed and in PATH.
- **Slow hot reload** → Use release mode: `flutter run -d chrome --release`.

---

## 8. References
- Flutter Official Docs: https://docs.flutter.dev
- Dart Language Overview: https://dart.dev
- Flutter Web Guide: https://docs.flutter.dev/platform-integration/web

---

## How to submit
- ZIP the project folder and attach it to your submission, or push the folder to GitHub and share the link.
- If submitting the document separately, export this README.md to PDF and upload.
