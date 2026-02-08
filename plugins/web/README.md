# Web Plugin

General web testing tools including browser automation, accessibility, and performance testing. Powered by [Playwright CLI](https://github.com/microsoft/playwright-cli).

## Prerequisites

- Node.js 18+ (install via mise, nvm, or directly)

## Installation

```bash
claude plugin install web@elias-plugins
```

## Setup

Install the Playwright CLI and browser:

```bash
npm install -g @playwright/cli@latest
playwright-cli install-browser
```

## Skills

### playwright-cli

Browser automation via CLI for web testing, form filling, screenshots, and data extraction. Includes reference docs for:

- Request mocking
- Running custom Playwright code
- Browser session management
- Storage state (cookies, localStorage)
- Test generation
- Tracing
- Video recording

### web-design-guidelines

UI code review against [Web Interface Guidelines](https://github.com/vercel-labs/agent-skills) from Vercel. 100+ rules covering accessibility, forms, animation, typography, performance, dark mode, and internationalization.
