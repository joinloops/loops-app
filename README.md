<p align="center"><a href="https://joinloops.org" target="_blank"><img src="https://raw.githubusercontent.com/joinloops/art/refs/heads/main/loops-logo-opticalsmall.png" width="200" alt="Loops Logo" style="border-radius:1rem;"></a></p>

# Loops Mobile App

This is the mobile app source that uses the [Loops](https://loops.video) service. 

### If you are looking to self-host Loops, please see the [loops-server](https://github.com/joinloops/loops-server) repository.

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

1. Install Node and necessary development tools:
```bash
# For macOS users (using Homebrew):
brew install node watchman
# Install JDK 17 if developing for Android
brew install --cask zulu17
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

  - Metro bundler cache issues:
  ```bash
  npm start -- --reset-cache
  ```

- For Android SDK issues, ensure your `ANDROID_HOME` environment variable is set correctly

## Funding

This project is funded through [NGI Zero Core](https://nlnet.nl/core), a fund established by [NLnet](https://nlnet.nl) with financial support from the European Commission's [Next Generation Internet](https://ngi.eu) program. Learn more at the [NLnet project page](https://nlnet.nl/project/Loops).

[<img src="https://nlnet.nl/logo/banner.png" alt="NLnet foundation logo" width="20%" />](https://nlnet.nl)
[<img src="https://nlnet.nl/image/logos/NGI0_tag.svg" alt="NGI Zero Logo" width="20%" />](https://nlnet.nl/core)

## Supporters

Thanks to the Fastly Fast Forward program, Fastly CDN and Object storage is used by Loops to host and serve Loops video to a global audience of people for free.

[<img src="https://github.com/user-attachments/assets/f1499b1f-c05f-480a-a5d5-dbebcb0e20fd" alt="Fastly Fast Forward logo" width="50%" />](https://www.fastly.com/fast-forward)
