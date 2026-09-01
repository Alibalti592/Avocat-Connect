# Avocat-Connect

Cross-platform mobile application connecting users with lawyers.

**React Native · Expo**

<!-- 📸 Add 3–5 screenshots here: onboarding/OTP, map/lawyer discovery, messaging.
     Drop the images in a /docs/screenshots folder and reference them:
     ![Lawyer discovery](docs/screenshots/discovery.png) -->

## Overview

Avocat-Connect lets users find and connect with lawyers through a map-based
discovery flow, with OTP-based authentication and in-app messaging.

## Features

- Authentication with OTP verification
- Profile creation
- Lawyer discovery via interactive maps and device location
- In-app messaging / conversation interface
- Navigation via React Navigation
- App-wide and auth state managed with Redux Toolkit
- Local persistence via AsyncStorage

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | React Native, Expo |
| Navigation | React Navigation |
| State | Redux Toolkit |
| Maps/Location | Expo Location + Maps |
| Local storage | AsyncStorage |
| Styling | Tailwind (NativeWind) |

*Note: this is currently a frontend-only mobile client. No backend/API repository is
included in this project.*

## Project Structure

```
Avocat-Connect/
├── Navigation/    # React Navigation setup
├── assets/        # Images, fonts, icons
├── components/    # Reusable UI components
├── redux/         # Redux Toolkit store, slices
├── screens/       # App screens
├── App.js         # Entry point
└── app.json       # Expo configuration
```

## Getting Started

### Prerequisites
- Node.js 18+
- Expo CLI (`npm install -g expo-cli`)
- Expo Go app (for testing on a physical device) or an emulator

### Installation

```bash
git clone https://github.com/Alibalti592/Avocat-Connect.git
cd Avocat-Connect

npm install   # or yarn install

cp .env.example .env
# fill in the values described below

npx expo start
```

## Environment Variables

Copy `.env.example` to `.env` and fill in real values before running the app.

| Variable | Purpose |
|---|---|
| `EXPO_PUBLIC_API_URL` | Base URL of the backend/API this app talks to, if any |
| `EXPO_PUBLIC_MAPS_API_KEY` | Maps provider API key used for lawyer discovery |
| `EXPO_PUBLIC_OTP_PROVIDER_KEY` | API key for the OTP/SMS verification provider |

*(Update this table with your project's real variable names if they differ — this is
a starting template based on standard Expo public-env conventions, not a claim about
your exact configuration.)*

## Roadmap / Future Improvements

- Add a documented backend/API layer
- Add automated tests
- Expand this README as backend work is added

## License

Personal project — license TBD.
