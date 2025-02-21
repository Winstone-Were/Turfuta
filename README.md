# Turfuta - Connecting People and Turfs

## Overview

Turfuta is an application designed to connect turf owners with people looking for turfs for various activities, such as sports, events, or other recreational purposes. The app allows users to find available turfs, book them, and communicate directly with the owners. The platform also provides real-time updates on turf availability and booking status.

## Features

- **User Authentication & Profiles**: Users can sign up, log in, and create profiles using Firebase Authentication.
- **Turf Listings**: Turf owners can list their turfs with details such as location, available facilities, pricing, and availability.
- **Real-Time Updates**: The app supports real-time updates using Firebase Realtime Database, ensuring users and owners are always informed about the status of bookings and turf availability.
- **Booking System**: Users can book turfs directly through the app, and owners can manage bookings easily.

## Tech Stack

- **Jetpack Compose**: For building the UI with a modern and reactive UI framework.
- **Firebase**: Used for authentication, database, and real-time updates.
  - Firebase Authentication for user login/sign-up
  - Firebase Realtime Database for real-time updates on turf availability and bookings
- **Kotlin**: Programming language for Android development.

## Screens

- **Home Screen**: Displays available turfs based on location and activity type.
- **Turf Details Screen**: Shows information about the selected turf, including availability, pricing, and facilities.
- **Profile Screen**: Users can view and update their profile details.
- **Booking Screen**: Allows users to make a booking for a turf.
- **Owner Dashboard**: Turf owners can manage their turf listings and view bookings.

## Run Instructions

To get the project running on your local machine, follow these steps:

### Prerequisites
- Android Studio installed (recommended version: 2023 or later)
- Firebase account and a Firebase project set up with Realtime Database and Authentication enabled
- Kotlin version 1.7 or later
- Jetpack Compose libraries included in your dependencies

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Winstone-Were/Turfuta
   ```

2. **Open the Project in Android Studio**
   - Launch Android Studio.
   - Select "Open an existing project" and navigate to the project folder.

3. **Set Up Firebase**
   - In Firebase Console, create a new project if you haven't already.
   - Add your Android app to the Firebase project and download the `google-services.json` file.
   - Place the `google-services.json` file in the `app/` directory of the project.

4. **Add Firebase SDK Dependencies**
   - Open the `build.gradle` file at the project level and ensure you have the required dependencies for Firebase:
     ```gradle
     classpath 'com.google.gms:google-services:4.3.10'  // Add this line
     ```
   - Open the `build.gradle` file at the app level and apply the Google services plugin:
     ```gradle
     apply plugin: 'com.google.gms.google-services'
     ```
   - Add Firebase SDK dependencies to the `dependencies` block:
     ```gradle
     implementation 'com.google.firebase:firebase-auth:21.0.3'
     implementation 'com.google.firebase:firebase-database:20.0.5'
     ```

5. **Sync Gradle**
   - Click on the "Sync Now" button in Android Studio to sync your Gradle files with Firebase.

6. **Run the App**
   - Connect your Android device or use an emulator.
   - Click on the green "Run" button in Android Studio or use the following command:
     ```bash
     ./gradlew assembleDebug
     ```

7. **Sign In and Test**
   - Use the Firebase authentication methods to log in (email/password, Google Sign-In, etc.).
   - Browse through the available turfs, make a booking, and test real-time updates.

---

## Contributing

Feel free to contribute to the project by submitting issues, feature requests, or pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
