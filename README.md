# Outdoorsman's Compass

Outdoorsman's Compass is an interactive web application designed for outdoor enthusiasts to seamlessly track, document, and explore wildlife sightings. Leveraging the power of Google Maps for precise geolocation and Firebase for secure data storage, the app enables users to log their observations, share images, and contribute to a dynamic, community-driven map of wildlife activity.

<img src="https://github.com/user-attachments/assets/1e9cdcf5-190d-4376-93d8-8564f3a8fc09" alt="Home Screen" width="600">

## Features

- **Pinpoint Coordinate System**: Uses Google Maps to display the user's location and submitted wildlife sightings.
- **User Authentication**: Google-based login/logout system.
- **Post Submissions**: Users can upload and post:
  - **Name of sighting**
  - **Pictures**
  - **Description**
- **Firebase Integration**: Stores and retrieves user submissions, including:
  - Post name
  - Picture
  - Description
  - Coordinates
  - User account details
- **User Profile and Map Integration**: Each user's submissions are linked to their profile and rendered on a shared Google Map.

## Project Structure

```
Outdoorsmans_Compass/
├── analysis_options.yaml
├── assets/
├── lib/
│   ├── firebase_options.dart
│   ├── main.dart
├── outdoorsmanscompass.iml
├── pubspec.lock
├── pubspec.yaml
├── web/
```
- assets/: Contains assets like images, icons, etc. 
- lib/: The main Flutter codebase, including Firebase configurations (firebase_options.dart) and application logic (main.dart). 
- web/: The folder with web-specific assets - for building and running the app in a browser. 
- analysis_options.yaml: Configuration for the Dart analysis options.

## Screenshots

### **User Submission Form**
<img src="https://github.com/user-attachments/assets/716da9b3-b252-406a-b4d7-3be179937be2" alt="User Submission" width="600">

### **Firebase Data Storage**
<img src="https://github.com/user-attachments/assets/d38dc773-48e8-46ae-8c63-2aa7647fd0a4" alt="Firebase Storage" width="600">

### **Submissions Overview**
<img src="https://github.com/user-attachments/assets/16c3cf02-2780-4916-af01-4bc9700005d7" alt="Submissions" width="600">

### **Map View with Wildlife Pins**
<img src="https://github.com/user-attachments/assets/c927a34c-c353-4a41-9724-191189f4fca2" alt="Wildlife Map" width="600">

## Dependencies
This project uses the following Flutter packages:
- [Flutter](https://flutter.dev/)
- [Firebase Core](https://pub.dev/packages/firebase_core)
- [Firebase Auth](https://pub.dev/packages/firebase_auth)
- [Cloud Firestore](https://pub.dev/packages/cloud_firestore)
- [Google Sign-In](https://pub.dev/packages/google_sign_in_web)
- [Google Maps](https://pub.dev/packages/google_maps_flutter)
- [Geolocator](https://pub.dev/packages/geolocator)
- [Image Picker](https://pub.dev/packages/image_picker)

## Setup and Installation

1. **Clone the Repository**
    ```sh
    git clone https://github.com/WilliamTLyons/OutdoorsmansCompass.git
    cd Outdoorsmans_Compass
    ```
2. **Install Flutter** ([Flutter](https://flutter-ko.dev/get-started/install))

3. **Install Dependencies**
   ```sh
   flutter pub get
   ```

4. **Run the Web Application**
   ```sh
   flutter run -d chrome
   ```

5. **Setup API Keys**
   - Add a **Google Maps API key** for map functionality.
   - Add a **Google Sign-In API key** for authentication.
   - Connect Firebase Firestore to store user submissions.

