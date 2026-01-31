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

## Plugins

### toolbox

A collection of commands and skills for everyday development tasks.

#### Commands

| Command | Description |
| ------- | ----------- |
| `git:commit-staged-changes` | Generate conventional commit messages for staged changes. Follows the conventional commits format with configurable types and scopes from `CLAUDE.md`. |

### react-native

Skills and commands to support React Native (Expo) development.

#### Skills

| Skill | Description |
| ----- | ----------- |
| `expo-troubleshoot` | Helps troubleshoot common Expo and React Native issues including build errors, runtime issues, and debugging. |
