# 📝 Animated ToDo App

A beautifully crafted, smoothly animated task management application built with React Native and Expo. This app features fluid animations, gesture-based interactions, and a modern user interface with dark mode support.

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![React Native](https://img.shields.io/badge/React%20Native-0.64.3-61dafb.svg)
![Expo](https://img.shields.io/badge/Expo-~43.0.2-000020.svg)

## ✨ Features

- **Smooth Animations**: Powered by Moti and React Native Reanimated for fluid, performant animations
- **Gesture-Based Interactions**: Swipe to delete tasks with intuitive gestures
- **Dark Mode Support**: Seamless theme switching with persistent color modes
- **Responsive Design**: Beautiful UI that adapts to different screen sizes
- **Task Management**: Create, edit, complete, and delete tasks
- **Animated Checkboxes**: Custom animated checkboxes with strike-through effects
- **Drawer Navigation**: Side drawer navigation for easy access to different screens
- **Cross-Platform**: Works on iOS, Android, and Web

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or later)
- [npm](https://www.npmjs.com/) or [Yarn](https://yarnpkg.com/)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)

For mobile development:

- [Expo Go](https://expo.dev/client) app on your iOS or Android device
- Or iOS Simulator (macOS) / Android Emulator

### Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/animated-todo-app.git
cd animated-todo-app
```

2. Install dependencies:

```bash
npm install
# or
yarn install
```

3. Start the development server:

```bash
npm start
# or
yarn start
```

4. Run on your preferred platform:

```bash
# iOS
npm run ios

# Android
npm run android

# Web
npm run web
```

## 🏗️ Project Structure

```
animated-todo-app/
├── assets/              # Images and static resources
├── src/
│   ├── assets/         # App-specific assets
│   ├── components/     # Reusable UI components
│   │   ├── animated-color-box.tsx
│   │   ├── animated-task-label.tsx
│   │   ├── app-container.tsx
│   │   ├── link-button.tsx
│   │   ├── masthead.tsx
│   │   ├── menu-button.tsx
│   │   ├── navbar.tsx
│   │   ├── sidebar.tsx
│   │   ├── swipable-view.tsx
│   │   ├── task-item.tsx
│   │   ├── task-list.tsx
│   │   └── theme-toggle.tsx
│   ├── screens/        # Screen components
│   │   ├── about-screen.tsx
│   │   └── main-screen.tsx
│   ├── utils/          # Utility functions and custom hooks
│   │   ├── styled.tsx
│   │   └── use-previous.ts
│   ├── index.tsx       # Navigation setup
│   └── theme.ts        # Theme configuration
├── App.tsx             # App entry point
├── app.json            # Expo configuration
├── package.json        # Dependencies and scripts
└── tsconfig.json       # TypeScript configuration
```

## 🛠️ Tech Stack

### Core Technologies

- **React Native** (0.64.3) - Cross-platform mobile framework
- **Expo** (~43.0.2) - Development platform for React Native
- **TypeScript** (~4.3.5) - Type-safe JavaScript

### UI & Styling

- **NativeBase** (^3.2.1) - Component library for consistent UI
- **Styled Components** (^5.3.3) - CSS-in-JS styling
- **Styled System** (^5.1.5) - Style props for components

### Animation

- **Moti** (^0.16.1) - Universal animation library
- **React Native Reanimated** (^2.2.4) - High-performance animations
- **React Native Gesture Handler** (^1.10.3) - Native gesture system

### Navigation

- **React Navigation** (^6.0.6) - Routing and navigation
- **React Navigation Drawer** (^6.1.8) - Drawer navigation

### Additional Libraries

- **React Native Checkbox Reanimated** (^0.1.0) - Animated checkboxes
- **React Native SVG** (^12.1.1) - SVG rendering
- **ShortID** (^2.2.16) - Unique ID generation

## 📱 Key Components

### TaskItem

Individual task component with:

- Animated checkbox with completion state
- Swipe-to-delete gesture
- Inline editing capability
- Strike-through animation for completed tasks

### TaskList

Manages the collection of tasks with:

- Add new tasks functionality
- Task state management
- List rendering with keys

### AnimatedColorBox

Custom animated container that:

- Supports theme transitions
- Provides smooth color changes
- Wraps content with animations

### Masthead

Header component featuring:

- Custom background image
- Gradient overlay
- Navigation integration

### ThemeToggle

Toggle component for:

- Dark/Light mode switching
- Persistent theme preference
- Smooth transition animations

## 🎨 Theming

The app uses NativeBase's theming system with custom color schemes. Theme configuration is defined in [src/theme.ts](src/theme.ts). The app supports both light and dark modes with smooth transitions.

## 📝 Scripts

| Command           | Description                       |
| ----------------- | --------------------------------- |
| `npm start`       | Start the Expo development server |
| `npm run android` | Run on Android device/emulator    |
| `npm run ios`     | Run on iOS simulator (macOS only) |
| `npm run web`     | Run in web browser                |
| `npm run eject`   | Eject from Expo (not recommended) |

## 🔧 Configuration

### Expo Configuration

The app configuration is managed in [app.json](app.json), including:

- App name and slug
- Icons and splash screens
- Platform-specific settings
- Asset bundle patterns

### TypeScript Configuration

TypeScript settings are in [tsconfig.json](tsconfig.json) with strict mode enabled for better type safety.

### Prettier Configuration

Code formatting rules are defined in [prettier.config.js](prettier.config.js) for consistent code style.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Expo team for the excellent development platform
- NativeBase for the comprehensive UI component library
- React Native community for the amazing ecosystem

## 📚 Resources

- [React Native Documentation](https://reactnative.dev/)
- [Expo Documentation](https://docs.expo.dev/)
- [NativeBase Documentation](https://docs.nativebase.io/)
- [Moti Animation Library](https://moti.fyi/)
- [React Navigation](https://reactnavigation.org/)

## 🐛 Known Issues

- None at the moment. If you find any bugs, please open an issue!

## 🗺️ Roadmap

- [ ] Add task categories/tags
- [ ] Implement task priorities
- [ ] Add due dates and reminders
- [ ] Cloud sync functionality
- [ ] Multi-language support
- [ ] Task search and filtering
- [ ] Statistics and productivity insights

---

Made with ❤️ by Erick Hernandez
