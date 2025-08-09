# School Tuck Shop App

An Android application for a School's tuck shop system, providing secure authentication and user management through Google Sign-In and Firebase.

## 🚧 Project Status

**⚠️ This project is currently under development and not yet complete.**

### ✅ Completed Features
- Google Sign-In Authentication
- Firebase Integration for user authentication
- User Profile Display (name and email)
- Session Management (auto-login for returning users)
- Secure Logout functionality

### 🔄 In Progress / Planned Features
- Tuck shop product catalog
- Shopping cart functionality
- Order management system
- Payment integration
- Admin panel for shop management
- Order history and tracking
- User preferences and settings

## 📱 Current Features

- **Google Sign-In Authentication**: Secure login using Google accounts
- **Firebase Integration**: Backend authentication and user management
- **User Profile Display**: Shows user name and email after successful login
- **Session Management**: Automatic login for returning users
- **Secure Logout**: Clean session termination

## 🏗️ Architecture

- **Language**: Java
- **Platform**: Android (API 17+)
- **Authentication**: Firebase Auth with Google Sign-In
- **UI Framework**: Android XML layouts with Material Design components

## 🛠️ Technologies Used

- **Android SDK**: Target SDK 30, Min SDK 17
- **Firebase Authentication**: Version 21.0.1
- **Google Play Services Auth**: Version 19.2.0
- **Material Design Components**: Version 1.4.0
- **AndroidX Libraries**: AppCompat, ConstraintLayout

## 📋 Prerequisites

Before running this application, ensure you have:

1. **Android Studio** (latest version recommended)
2. **Java Development Kit (JDK)** 8 or higher
3. **Google Services JSON file** (`google-services.json`) configured for your project
4. **Firebase project** set up with Authentication enabled
5. **Google Sign-In** configured in Firebase Console

## 🚀 Installation & Setup

### 1. Clone the Repository
```bash
git clone <repository-url>
cd School-Tuck-Shop-App
```

### 2. Firebase Configuration
1. Go to the [Firebase Console](https://console.firebase.google.com/)
2. Create a new project or select existing one
3. Add an Android app to your project
4. Use package name: `com.example.amstuckshopapp`
5. Download the `google-services.json` file
6. Place it in the `app/` directory

### 3. Enable Authentication
1. In Firebase Console, go to Authentication > Sign-in method
2. Enable Google Sign-In provider
3. Add your app's SHA-1 fingerprint

### 4. Build and Run
1. Open the project in Android Studio
2. Sync the project with Gradle files
3. Connect an Android device or start an emulator
4. Click "Run" or use `Ctrl+R`

## 📱 Current App Structure

```
app/src/main/
├── java/com/example/amstuckshopapp/
│   ├── SignIn.java          # Main authentication activity
│   └── homePage.java        # User dashboard after login
├── res/
│   ├── layout/
│   │   ├── activity_sign_in.xml    # Sign-in screen layout
│   │   └── activity_main.xml       # Home page layout
│   └── values/
│       └── strings.xml             # App strings and resources
└── AndroidManifest.xml             # App configuration
```

## 🔐 Authentication Flow

1. **App Launch**: User lands on Sign-In screen
2. **Check Session**: App checks if user is already authenticated
3. **Google Sign-In**: User taps sign-in button to authenticate with Google
4. **Firebase Auth**: Google token is used to authenticate with Firebase
5. **Home Screen**: Successfully authenticated users see the home page
6. **Logout**: Users can sign out, which clears the session

## 🎨 Current User Interface

- **Sign-In Screen**: Clean interface with Google Sign-In button
- **Home Screen**: Basic welcome screen displaying user's name and email
- **Material Design**: Modern Android UI following Material Design principles

*Note: The UI is currently minimal and will be expanded as more features are implemented.*

## 🔧 Configuration

### Key Configuration Files:
- `build.gradle` (Module: app): Dependencies and build configuration
- `google-services.json`: Firebase project configuration
- `AndroidManifest.xml`: App permissions and activity declarations

### Important Dependencies:
```gradle
implementation 'com.google.firebase:firebase-auth:21.0.1'
implementation 'com.google.android.gms:play-services-auth:19.2.0'
implementation 'androidx.appcompat:appcompat:1.3.1'
implementation 'com.google.android.material:material:1.4.0'
```


## 🐛 Troubleshooting

### Common Issues:

1. **Sign-In Failed**: 
   - Ensure `google-services.json` is properly configured
   - Check SHA-1 fingerprint in Firebase Console
   - Verify Google Sign-In is enabled in Firebase Authentication

2. **Build Errors**:
   - Sync project with Gradle files
   - Check internet connection for dependency downloads
   - Ensure Android SDK is up to date

3. **Authentication Issues**:
   - Verify Firebase project configuration
   - Check if Google Play Services are installed on device/emulator


## 📝 Development Notes

This is an ongoing school project for a school. The current version only includes basic authentication functionality. More features will be added as development progresses.


**Package Name**: `com.example.amstuckshopapp`  
**Version**: 1.0 (Development)  
**Target SDK**: 30  
**Min SDK**: 17
 
