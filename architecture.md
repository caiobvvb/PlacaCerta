# PlacaCerta - Car Plate Photo Capture App

## Overview
A lightweight Android app for capturing car plate photos with Google authentication and cloud storage integration.

## Core Features
1. Brazilian car plate input (format validation)
2. Camera integration for photo capture
3. Google authentication
4. Photo storage in Google Drive, local device, and server
5. Elegant, modern UI with vibrant colors and generous spacing

## Technical Architecture

### File Structure
- `main.dart` - App entry point
- `theme.dart` - Modern color scheme with vibrant colors
- `screens/`
  - `home_screen.dart` - Main screen with plate input
  - `camera_screen.dart` - Camera capture interface
  - `photo_gallery_screen.dart` - View captured photos
  - `login_screen.dart` - Google authentication
- `models/`
  - `plate_photo.dart` - Data model for plate photos
- `services/`
  - `auth_service.dart` - Google authentication
  - `camera_service.dart` - Camera operations
  - `storage_service.dart` - Local and cloud storage
- `widgets/`
  - `plate_input_field.dart` - Custom Brazilian plate input
  - `custom_button.dart` - Styled buttons
- `utils/`
  - `validators.dart` - Plate format validation
  - `constants.dart` - App constants

### Data Models
- PlatePhoto: id, plateNumber, imagePath, timestamp, isUploaded

### Dependencies Required
- camera: Camera functionality
- image_picker: Additional image handling
- google_sign_in: Google authentication
- googleapis: Google Drive API
- path_provider: Local file paths
- shared_preferences: Local data persistence
- permission_handler: Camera permissions

### UI Design
- Vibrant color palette (avoiding Material Design)
- Generous spacing and padding
- Sophisticated typography using Google Fonts
- Modern, clean interface with custom animations

## Implementation Steps
1. Update theme with vibrant colors
2. Add required dependencies
3. Create data models
4. Implement authentication service
5. Build main screens (Login, Home, Camera, Gallery)
6. Add camera functionality
7. Implement storage services
8. Add Brazilian plate validation
9. Create custom UI components
10. Test and compile project