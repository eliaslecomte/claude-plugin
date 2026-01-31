---
name: expo-troubleshoot
description: Helps troubleshoot common Expo and React Native issues. Use when the user encounters build errors, runtime issues, or needs help debugging their Expo app.
---

# Expo Troubleshooting

Help the user troubleshoot common Expo and React Native issues.

## Guidelines

- Ask clarifying questions about the error message or behavior
- Check for common causes first (dependencies, config, cache)
- Suggest clearing caches when appropriate (`npx expo start -c`, `watchman watch-del-all`)
- Reference Expo documentation when relevant

## Common Issues to Check

### Build/Start Issues
- Node modules need reinstalling (`rm -rf node_modules && npm install`)
- Expo cache needs clearing (`npx expo start -c`)
- Metro bundler cache (`npx expo start --clear`)
- Watchman issues (`watchman watch-del-all`)

### Native Module Issues
- Check if the module supports Expo Go vs requires a development build
- Verify expo-dev-client is installed for custom native code
- Check compatibility with current Expo SDK version

### Configuration
- Verify app.json/app.config.js settings
- Check babel.config.js for required plugins
- Ensure metro.config.js is properly configured

## Debugging Steps

1. Identify the error type (build, runtime, native)
2. Check recent changes that may have caused the issue
3. Verify dependencies are compatible with Expo SDK version
4. Suggest specific fix based on error pattern
