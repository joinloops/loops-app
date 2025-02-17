<p align="center"><a href="https://joinloops.org" target="_blank"><img src="https://raw.githubusercontent.com/joinloops/art/refs/heads/main/logo.png" width="200" alt="Loops Logo" style="border-radius:1rem;"></a></p>

# Loops Mobile App

This is the mobile app source that uses the [Loops](https://loops.video) service.

## Prerequisites
* Node.js (version 16 or newer)
* npm or yarn package manager
* Git

## iOS Development Requirements (macOS only)
* Xcode (latest version recommended)
* CocoaPods (`sudo gem install cocoapods`)
* macOS

## Android Development Requirements
* Android Studio
* Android SDK
* Java Development Kit (JDK) 11 or newer

## Installation Steps

1. Install React Native CLI globally:
```bash
npm install -g react-native-cli
```

2. Clone your loops app repository:
```bash
git clone https://github.com/joinloops/loops-app
cd loops-app
```

3. Install dependencies:
```bash
npm install
# or if using yarn
yarn install
```

4. iOS Setup (macOS only):
```bash
cd ios
pod install
cd ..
```

5. Start Metro Bundler:
```bash
npx react-native start
```

6. Run the app:

For iOS (macOS only):
```bash
npx react-native run-ios
```

For Android:
```bash
npx react-native run-android
```

## Common Issues and Solutions

- If you encounter any build errors, try cleaning the build:
  ```bash
  # For iOS
  cd ios
  pod deintegrate
  pod install
  cd ..

  # For Android
  cd android
  ./gradlew clean
  cd ..
  ```

- For Android SDK issues, ensure your `ANDROID_HOME` environment variable is set correctly