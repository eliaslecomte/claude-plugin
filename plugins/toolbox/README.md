# Toolbox Plugin

A collection of commands and skills for everyday development tasks.

## Installation

```bash
claude plugin install toolbox@elias-plugins
```

## Commands

### git:commit-staged-changes

Generate conventional commit messages for staged changes. Follows the conventional commits format with configurable types and scopes.

#### Setup

Add a scopes table to your project's `CLAUDE.md` to define allowed scopes:

```markdown
## Git Commit Scopes

| Scope | Description                |
| ----- | -------------------------- |
| api   | API and backend changes    |
| ui    | User interface components  |
| core  | Core business logic        |
```

#### Commit Types

| Type     | Description                           |
| -------- | ------------------------------------- |
| feat     | New feature                           |
| fix      | Bug fix                               |
| chore    | Maintenance (e.g., tooling, deps)     |
| docs     | Documentation changes                 |
| refactor | Code restructure (no behavior change) |
| test     | Adding or refactoring tests           |
| style    | Code formatting (no logic change)     |
| perf     | Performance improvements              |
