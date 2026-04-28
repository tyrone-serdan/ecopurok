# BasuraSmart

A waste management mobile application built with Expo and React Native.

## Overview

BasuraSmart is designed to help communities manage their waste collection more efficiently. The app provides a streamlined experience for both residents and garbage collectors, making it easier to track pickup schedules, view routes, and ensure proper waste segregation.

## Features

### For Residents
- View monthly pickup schedule calendar
- Get reminders for upcoming waste collection days
- Color-coded waste type indicators (biodegradable, non-biodegradable, recyclables)
- Access to waste segregation guidelines

### For Collectors
- View assigned pickup routes with all stops
- Track completed and pending stops
- Mark individual pickups as complete
- See route progress in real-time

### Authentication
- Phone-based registration and login
- OTP verification for account security
- Secure session management with Zustand

## Tech Stack

- **Framework:** Expo SDK 52 with Expo Router
- **Language:** TypeScript
- **State Management:** Zustand
- **Styling:** React Native StyleSheet
- **Navigation:** Expo Router (file-based routing)
- **UI Components:** Custom components with React Native SVG

## Getting Started

### Prerequisites

- Node.js 18+
- npm or yarn
- Expo CLI
- Android Studio (for Android development)
- Xcode (for iOS development, macOS only)

### Installation

```bash
# Install dependencies
npm install

# Start the development server
npm start

# Run on Android
npm run android

# Run on iOS
npm run ios
```

## Demo Credentials

The app uses mock data for demonstration purposes:

| User Type | Username | Password |
|-----------|----------|----------|
| Resident | resident | demo123 |
| Collector | collector | demo123 |

### OTP Code
Use `123456` for OTP verification during registration.

## Project Structure

```
basurasmart/
├── app/                    # Expo Router screens
│   ├── (auth)/            # Authentication screens
│   │   ├── login.tsx
│   │   ├── register.tsx
│   │   ├── otp.tsx
│   │   └── details.tsx
│   ├── (resident)/        # Resident screens
│   │   └── home.tsx
│   ├── (collector)/       # Collector screens
│   │   └── route.tsx
│   ├── _layout.tsx        # Root layout
│   └── index.tsx          # Landing page
├── components/            # Reusable components
│   ├── ui/               # UI components
│   └── illustrations/    # SVG illustrations
└── lib/                  # Utilities and logic
    ├── api.ts            # API functions (mock)
    ├── constants.ts      # App constants
    ├── store.ts         # Zustand stores
    ├── styles.ts        # Shared styles
    └── types.ts         # TypeScript types
```
