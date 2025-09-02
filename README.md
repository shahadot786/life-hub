# LifeHub - Smart Finance & Task Manager

A comprehensive cross-platform mobile and web application for managing tasks and finances, built with Expo and React Native.

## Features

### 🔐 Authentication

- Email/password authentication
- Secure user sessions
- Password reset functionality

### 📋 Task Management

- Create, edit, and delete tasks
- Priority levels (low, medium, high)
- Due date tracking
- Streak counter for motivation
- Points system for gamification

### 💰 Finance Tracking

- Income and expense tracking
- Category-based organization
- Monthly spending analysis
- Savings goals tracking
- Visual charts and progress indicators

### 🎯 Gamification

- Points for completed tasks
- Achievement system
- Daily streak tracking
- Progress visualization

### 🎨 Modern UI/UX

- Material Design 3 theming
- Dark/light mode support
- Smooth animations and transitions
- Responsive design for all screen sizes

## Tech Stack

- **Framework**: Expo (React Native)
- **Navigation**: Expo Router
- **State Management**: Zustand with persistence
- **UI Library**: React Native Paper
- **Forms**: React Hook Form + Yup validation
- **Animations**: React Native Reanimated
- **Charts**: React Native Chart Kit
- **Storage**: AsyncStorage for offline support

## Architecture

### Modular Structure

```
LifeHub/
│
├── app/                        # Expo Router (screens & navigation)
│   ├── _layout.tsx             # Root layout (wrap with Provider, Theme, etc.)
│   ├── (tabs)/                 # Tab-based navigation
│   │   ├── _layout.tsx         # Tab layout file
│   │   ├── index.tsx           # Home/Dashboard tab
│   │   ├── tasks.tsx           # Task management tab
│   │   ├── finance.tsx         # Finance/Expense tab
│   │   ├── profile.tsx         # Profile tab
│   │   └── settings.tsx        # Settings tab
│   │
│   ├── auth/                   # Stack for auth screens
│   │   ├── login.tsx
│   │   ├── signup.tsx
│   │   └── forgot-password.tsx
│   │
│   └── onboarding.tsx          # First-time user onboarding
│
├── src/                        # Core business logic
│   ├── components/             # Reusable UI components
│   │   ├── ui/                 # Button, Input, Card, etc.
│   │   ├── charts/             # Charts/Graphs
│   │   └── layout/             # Header, TabBar, etc.
│   │
│   ├── features/               # Feature-based modules
│   │   ├── tasks/              # Task module
│   │   │   ├── api.ts
│   │   │   ├── store.ts
│   │   │   └── types.ts
│   │   ├── finance/            # Finance module
│   │   │   ├── api.ts
│   │   │   ├── store.ts
│   │   │   └── types.ts
│   │   ├── profile/
│   │   └── auth/
│   │
│   ├── hooks/                  # Custom hooks
│   ├── lib/                    # Helpers/utilities
│   ├── services/               # API, DB, Notifications
│   ├── store/                  # Global Zustand stores
│   ├── theme/                  # Theme system
│   ├── types/                  # Global types/interfaces
│   └── config/                 # App config/constants
│
├── assets/                     # Images, fonts, icons, lotties
│
├── scripts/                    # CI/CD, seeding, automation
│
├── app.json
├── babel.config.js
├── tsconfig.json
└── package.json

```

### State Management

- **AuthStore**: User authentication and session management
- **TaskStore**: Task CRUD operations and streak tracking
- **FinanceStore**: Transaction and savings goal management
- **ThemeStore**: Dark/light mode preferences

### Offline Support

- All data persisted locally using AsyncStorage
- Offline-first architecture ready for sync capabilities
- State persistence across app restarts

## Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for web
npm run build:web
```

## Platform Support

- **iOS**: Full native support
- **Android**: Full native support
- **Web**: Responsive web app with all features

## Future Enhancements

- Backend integration (Firebase/Supabase)
- Real-time data synchronization
- Social features and sharing
- Advanced analytics and insights
- Premium features with Stripe integration
- AI-powered financial advice
- Cloud backup and restore

## Contributing

This project follows modern React Native best practices with TypeScript, modular architecture, and comprehensive testing setup.
