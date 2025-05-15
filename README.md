# sync_xp

To Able start work/run this application, make sure you have finished all the installation for the tools that it need to run this application:

Windows User:
1) Visual Studio Code
2) Flutter sdk (when extract the file do not extract to  C\Program Files)
3) git
4) Android studio (Emulator)
5) Extension that need to install in Visual Studio Code
 - Dart
 - Flutter
 - Awesone flutter snippets
 - Bracket Pair Colorizer
 - Material Icon theme (optional)

Mac User:
1) Flutter SDK 
2) Android Studiio
3) Git
4) Visual Studio Code
5) Extension that need to be install in Visual Studio Code
 - Dart
 - Flutter
 - Awesome Flutter Snippets
 - Bracket pair colorizer
 - Material Icon Theme (optional)
 - Xcode and simulator (Can be install at App Store)

 How to install? What was the process?
https://www.youtube.com/watch?v=CD1Y2DmL5JM&t=867s

This link include the installation process for both Mac and Windows User, and also some basic tutorial.

## Getting Started

Project Structure (Tree Diagram)


lib/
├── main.dart
|
├── app/
│   ├── app.dart
│   └── router.dart
|   
├── core/
│   ├── constants/           # Colors, text, icons
│   ├── utils/               # Reusable helpers
│   └── services/            # General-purpose services (e.g., mock DB, location)
|
├── mock_data/               # Local mock data (users, events)
|
├── models/                  # UserModel, EventModel, MatchModel
|
├── controller/
│   ├── matchmaking_controller.dart
│   ├── event_controller.dart
│   ├── onboarding_controller.dart
│   └── profile_controller.dart
|
├── features/
|   |
│   ├── onboarding/
│   │   ├── views/
│   │   └── widgets/
|   |
│   ├── profile/
│   │   ├── views/
│   │   └── widgets/
|   |
│   ├── matchmaking/
│   │   ├── views/
│   │   └── widgets/
|   |
│   └── events/
│       ├── views/
│       └── widgets/
|
├── providers/               # Riverpod, Bloc, or other state logic
└── widgets/                 # Reusable components (cards, chips, etc.)



## 🧠 Controller Directory

All core logic and business rules live in the `lib/controller/` directory. This includes:

- **MatchmakingController**: Handles compatibility scoring and suggested athlete lists.
- **EventController**: Filters and returns relevant nearby sporting events.
- **ProfileController**: Manages user data, onboarding steps, and preferences.
- **OnboardingController**: Handles onboarding form state and validation.

This keeps the `features/` directory clean and focused purely on UI components like screens (`views/`) and UI parts (`widgets/`).
