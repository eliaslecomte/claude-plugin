# My Claude Toolbox

A personal collection of commands and skills for [Claude Code](https://docs.anthropic.com/en/docs/claude-code).

## Installation

Add the marketplace and install the plugin:

```
/plugin marketplace add eliaslecomte/claude-plugin
/plugin install toolbox@elias-plugins
```

## Setup

### Commit Scopes

The `git:commit-staged-changes` command reads commit scopes from your project's `CLAUDE.md` file. Add a scopes table to define the allowed scopes for your project:

```markdown
## Git Commit Scopes

| Scope     | Description                           |
| --------- | ------------------------------------- |
| api       | API and backend changes               |
| ui        | User interface components             |
| core      | Core business logic                   |
```

## Recommended Complementary Plugins

### General Development

| Plugin | Description | Install |
| ------ | ----------- | ------- |
| [Superpowers](https://github.com/obra/superpowers) | Complete dev workflow with design, planning, execution, and verification phases | `/plugin marketplace add obra/superpowers-marketplace`<br>`/plugin install superpowers@superpowers-marketplace` |

## Plugins

### toolbox

A collection of commands and skills for everyday development tasks.

#### Commands

| Command | Description |
| ------- | ----------- |
| `git:commit-staged-changes` | Generate conventional commit messages for staged changes. Follows the conventional commits format with configurable types and scopes from `CLAUDE.md`. |

### react

React and Next.js best practices, performance optimization, and composition patterns. Skills sourced from [Vercel Agent Skills](https://github.com/vercel-labs/agent-skills).

#### Skills

| Skill | Description |
| ----- | ----------- |
| `react-best-practices` | 40+ React/Next.js performance optimization rules across 8 categories. |
| `composition-patterns` | Composition patterns for scalable React components: compound components, state lifting, explicit variants. |

### react-native

Skills and commands to support React Native (Expo) development.

#### Skills

| Skill | Description |
| ----- | ----------- |
| `expo-troubleshoot` | Helps troubleshoot common Expo and React Native issues including build errors, runtime issues, and debugging. |
| `react-native-skills` | 35+ React Native/Expo best practices from Vercel covering performance, layout, animations, and platform patterns. |

### web

General web testing tools including browser automation, accessibility, and performance testing. Powered by [Playwright CLI](https://github.com/microsoft/playwright-cli).

#### Setup

Install the Playwright CLI and browser:

```bash
npm install -g @playwright/cli@latest
playwright-cli install-browser
```

#### Skills

| Skill | Description |
| ----- | ----------- |
| `playwright-cli` | Browser automation via CLI for web testing, form filling, screenshots, data extraction, and test generation. |
| `web-design-guidelines` | UI code review against Web Interface Guidelines from Vercel. 100+ rules for accessibility, performance, and UX. |
