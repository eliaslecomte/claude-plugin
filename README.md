# My Claude Toolbox

A personal collection of commands and skills for [Claude Code](https://docs.anthropic.com/en/docs/claude-code).

## Installation

Clone the repository:

```bash
git clone https://github.com/eliaslecomte/claude-plugin.git
```

Then add the path to your `~/.claude/settings.json`:

```json
{
  "plugins": ["/path/to/claude-plugin"]
}
```

## Available Commands

- `commit-staged-changes` - Generate conventional commit messages for staged git changes
