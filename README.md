<h1>
  <img src="appicon.png" alt="Logo" style="height:35px; vertical-align: middle;">
  RunningTrackerApp - Advanced Fitness Activity Tracker
</h1>


RunningTrackerApp is a sophisticated Android fitness tracking application built with modern technologies including Jetpack Compose, MVVM architecture, and Google Maps integration. The app enables users to monitor their running activities in real-time, visualize routes on interactive maps, and maintain comprehensive activity statistics using Room database persistence.


## Key Features

- **Real-time GPS Tracking**: Monitor your running activities with precise GPS tracking
- **Interactive Route Visualization**: View your running path in real-time using the Google Maps Compose library
- **Background Tracking**: Continuous activity monitoring via Foreground Service, even when the app is closed or removed from the background
- **Comprehensive Data Storage**: Persistent storage of running statistics with Room database
- **Advanced Navigation**: Seamless nested navigation, deep linking, and conditional navigation to onboarding screens via Jetpack Navigation Component
- **Permission-free Image Selection**: Integrated Jetpack Compose image picker for hassle-free image selection without additional permissions
- **Efficient Data Loading**: Integrated Paging3 for smooth, efficient data presentation

## Getting Started

### Basic Setup
1. Clone the repository
```
git clone https://github.com/adityaxxz/RunningTrackerApp
```
3. Open the project in Android Studio

<!-- <img src="" alt="" width="400px"> -->

<!-- ### Google Maps Integration (Optional)
The core tracking functionality works without Maps integration, but for the full experience:

1. Obtain a Google Maps API key following the official [guide](https://developers.google.com/maps/documentation/android-sdk/get-api-key)
2. Open the `local.properties` file
3. Add your API key:
   ```
   MAPS_API_KEY=your_maps_api_key
   ``` -->

## Screenshots

<div style="display: flex; gap: 20px;">
  <img src="./ss/ss1.png" alt="RunningTrackerApp_live_tracking_ss" width="325px">
  <img src="./ss/ss3.png" alt="run_track_statistics_ss" width="300px">
  <img src="./ss/ss4.png" alt="run_track_statistics_ss" width="300px">
  <img src="./ss/ss5.png" alt="run_track_statistics_ss" width="300px">
</div>

## Architecture & Package Structure

RunningTrackerApp follows the MVVM architecture with Unidirectional Data Flow (UDF) and clean architecture principles. The project is organized into the following key packages:

* **`background`**: Manages background processes including services
* **`data`**: Responsible for data production and management
    * **`tracking`**: Handles location tracking and activity monitoring
* **`di`**: Contains Hilt dependency injection modules
* **`domain`**: Houses common use cases and interfaces
* **`ui`**: Manages the application's user interface
    * **`nav`**: App navigation and destination management
    * **`screen`**: UI implementation components
    * **`theme`**: Material 3 theming components
    * **`common`**: UI utilities and shared components
* **`common`**: Cross-application utility classes

## Technology Stack

- **[Kotlin](https://kotlinlang.org/)**: Modern, concise programming language
- **[Jetpack Compose](https://developer.android.com/jetpack/compose)**: Declarative UI framework
- **[Jetpack Navigation](https://developer.android.com/jetpack/compose/navigation)**: Screen navigation and deep linking
- **[Google Maps API](https://developers.google.com/maps/documentation/android-sdk)**: Location tracking and map visualization
