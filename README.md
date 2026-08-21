# Gluestack UI + Expo SDK 54 Preset (Uniwind & Tailwind CSS v4)

A modern, production-ready Expo SDK 54 starter preset powered by **Gluestack UI**, **Uniwind**, **Tailwind CSS v4**, and **React Native New Architecture**.

---

## Features

- ⚡ **Expo SDK 54**: Latest Expo runtime with React Native 0.81 & React 19.
- 🚀 **New Architecture Enabled**: Built with `newArchEnabled: true` out of the box.
- 🎨 **Gluestack UI + Uniwind**: Fast, customizable, and accessible cross-platform UI components styled with Tailwind CSS v4.
- 🧭 **Expo Router v6**: File-based routing with typed routes support.
- 🌗 **Light / Dark Mode**: Built-in theme switcher with `GluestackUIProvider` and `StatusBar` management.
- 📱 **Cross-Platform**: Support for iOS, Android, and Web with SSR static rendering.
- 📐 **Safe Area Integration**: Uniwind + `react-native-safe-area-context` integration.
- 🔤 **Lucide Icons**: Crisp, vector icon library via `lucide-react-native`.

---

## Quick Start

### 1. Clone or Use This Template
```bash
git clone <YOUR_REPO_URL> my-app
cd my-app
```

### 2. Install Dependencies
```bash
yarn install
# or
npm install
```

### 3. Start the Development Server
```bash
yarn start
```

---

## Available Scripts

| Command | Description |
| :--- | :--- |
| `yarn start` | Starts the Expo development server |
| `yarn dev` | Starts the Expo dev server and resets bundler cache |
| `yarn ios` | Runs the app on iOS Simulator |
| `yarn android` | Runs the app on Android Emulator |
| `yarn web` | Starts the web development server |
| `yarn typecheck` | Runs TypeScript compiler type check (`tsc --noEmit`) |

---

## Project Structure

```text
├── app/                        # Expo Router file-based navigation
│   ├── _layout.tsx             # Root layout with Providers & theme management
│   └── index.tsx               # Home screen
├── components/
│   ├── custom/                 # Custom user components (e.g. ThemeSwitcher)
│   └── ui/                     # Gluestack UI primitive components
├── global.css                  # Global Tailwind CSS v4 stylesheets & design tokens
├── metro.config.js             # Metro bundler config with Uniwind integration
├── babel.config.js             # Babel config with module aliases & worklets
├── app.json                    # Expo project configuration (SDK 54)
├── tsconfig.json               # TypeScript path alias configuration (@/*)
└── uniwind-types.d.ts          # Uniwind type declarations
```

---

## Theming & Styling

This preset uses **Tailwind CSS v4** via **Uniwind**. Design tokens and color schemes are defined in `global.css`.

### Using Theme Tokens in Components:
```tsx
import { View, Text } from 'react-native';
import { Button, ButtonText } from '@/components/ui/button';

export default function Example() {
  return (
    <View className="flex-1 bg-background p-4 items-center justify-center">
      <Text className="text-2xl font-bold text-foreground mb-4">
        Hello World
      </Text>
      <Button size="default">
        <ButtonText>Get Started</ButtonText>
      </Button>
    </View>
  );
}
```

---

## Health Checks

Verify your environment and dependencies:
```bash
npx expo-doctor
```

---

## License

MIT
