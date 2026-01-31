# React Native Plugin

Skills and commands to support React Native (Expo) development.

## Installation

```bash
claude plugin install react-native@elias-plugins
```

## Recommended: Vercel Agent Skills

This plugin focuses on Expo-specific workflows. For comprehensive React Native best practices, also install the Vercel agent skills:

```bash
npx skills add vercel-labs/agent-skills
```

This adds `react-native-guidelines` and `react-best-practices` skills that complement this plugin.

## Skills

### expo-troubleshoot

Helps troubleshoot common Expo and React Native issues including:

- Build and start issues (cache, Metro bundler, Watchman)
- Native module compatibility (Expo Go vs development builds)
- Configuration problems (app.json, babel.config.js, metro.config.js)
