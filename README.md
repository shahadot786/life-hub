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
├── app/                    # Expo Router screens
│   ├── (auth)/            # Authentication screens
│   └── (tabs)/            # Main app tabs
├── components/            # Reusable UI components
├── store/                 # Zustand stores
├── services/              # API and utility services
├── contexts/              # React contexts
├── types/                 # TypeScript definitions
├── utils/                 # Helper functions
└── constants/             # App constants
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
