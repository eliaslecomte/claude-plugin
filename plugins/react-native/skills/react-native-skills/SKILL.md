---
name: react-native-skills
description: React Native and Expo best practices for building performant mobile apps
license: MIT
metadata:
  author: vercel
  version: '1.0.0'
---

# React Native Skills

React Native and Expo best practices for building performant mobile apps.

## When to Apply

- Building React Native or Expo applications
- Optimizing list and scroll performance
- Implementing animations with Reanimated
- Working with images and media
- Configuring native modules or fonts
- Structuring monorepo projects with native dependencies

## Rule Categories by Priority

| Priority | Category | Rules |
|----------|----------|-------|
| CRITICAL | List Performance | `list-performance-virtualize`, `list-performance-item-memo`, `list-performance-callbacks`, `list-performance-inline-objects`, `list-performance-function-references`, `list-performance-images`, `list-performance-item-expensive`, `list-performance-item-types` |
| HIGH | Animation | `animation-gpu-properties`, `animation-derived-value`, `animation-gesture-detector-press` |
| HIGH | Navigation | `navigation-native-navigators` |
| HIGH | UI Patterns | `ui-expo-image`, `ui-image-gallery`, `ui-pressable`, `ui-safe-area-scroll`, `ui-scrollview-content-inset`, `ui-menus`, `ui-native-modals`, `ui-measure-views`, `ui-styling` |
| MEDIUM | State Management | `react-state-minimize`, `react-state-dispatcher`, `react-state-fallback`, `react-compiler-destructure-functions`, `react-compiler-reanimated-shared-values` |
| MEDIUM | Rendering | `rendering-text-in-text-component`, `rendering-no-falsy-and` |
| MEDIUM | Monorepo | `monorepo-native-deps-in-app`, `monorepo-single-dependency-versions` |
| LOW | Configuration | `fonts-config-plugin`, `imports-design-system-folder`, `js-hoist-intl` |

## Quick Reference

### List Performance (CRITICAL)

- **list-performance-virtualize** — Use FlashList for large lists
- **list-performance-item-memo** — Memoize list item components
- **list-performance-callbacks** — Stabilize callback references
- **list-performance-inline-objects** — Avoid inline style objects
- **list-performance-function-references** — Extract functions outside render
- **list-performance-images** — Optimize images in lists
- **list-performance-item-expensive** — Move expensive work outside items
- **list-performance-item-types** — Use item types for heterogeneous lists

### Animation (HIGH)

- **animation-gpu-properties** — Animate only transform and opacity
- **animation-derived-value** — Use useDerivedValue for computed animations
- **animation-gesture-detector-press** — Use Gesture.Tap instead of Pressable

### Navigation (HIGH)

- **navigation-native-navigators** — Use native stack and native tabs over JS navigators

### UI Patterns (HIGH)

- **ui-expo-image** — Use expo-image for optimized images
- **ui-image-gallery** — Use Galeria for image galleries and lightbox
- **ui-pressable** — Use Pressable instead of Touchable components
- **ui-safe-area-scroll** — Use contentInsetAdjustmentBehavior for safe areas
- **ui-scrollview-content-inset** — Use contentInset for dynamic ScrollView spacing
- **ui-menus** — Use native menus for dropdowns and context menus
- **ui-native-modals** — Use native modals over JS-based bottom sheets
- **ui-measure-views** — Measuring view dimensions
- **ui-styling** — Modern React Native styling patterns

### State Management (MEDIUM)

- **react-state-minimize** — Minimize state variables and derive values
- **react-state-dispatcher** — useState dispatch updaters for state that depends on current value
- **react-state-fallback** — Use fallback state instead of initialState
- **react-compiler-destructure-functions** — Destructure functions early in render (React Compiler)
- **react-compiler-reanimated-shared-values** — Use .get() and .set() for Reanimated shared values (not .value)

### Rendering (MEDIUM)

- **rendering-text-in-text-component** — Wrap strings in Text components
- **rendering-no-falsy-and** — Never use && with potentially falsy values

### Monorepo (MEDIUM)

- **monorepo-native-deps-in-app** — Install native dependencies in app directory
- **monorepo-single-dependency-versions** — Use single dependency versions across monorepo

### Configuration (LOW)

- **fonts-config-plugin** — Load fonts natively at build time
- **imports-design-system-folder** — Import from design system folder
- **js-hoist-intl** — Hoist Intl formatter creation

## How to Use

Individual rule files are located in the `rules/` directory. Each rule file contains:

- Detailed explanation of the rule
- Incorrect code examples (what to avoid)
- Correct code examples (what to do)
- Additional context and references

## Full Compiled Document

For the complete expanded guide with all rules, explanations, and code examples, see [AGENTS.md](./AGENTS.md).
