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

### React Native Development

Use alongside the **react-native** plugin:

| Plugin | Description | Install |
| ------ | ----------- | ------- |
| [Vercel Agent Skills](https://github.com/vercel-labs/agent-skills) | React and React Native best practices (40+ rules), includes `react-native-guidelines` and `react-best-practices` | `npx skills add vercel-labs/agent-skills` |

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
