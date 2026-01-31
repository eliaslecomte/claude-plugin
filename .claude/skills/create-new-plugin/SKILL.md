---
name: create-new-plugin
description: Instructions for creating a new Claude plugin in this marketplace repository. Use when the user wants to create, scaffold, or set up a new plugin.
---

# Create a new Claude plugin

Your task is to help the user create a new Claude plugin in this marketplace repository.

## Guidelines

- Ask the user for the plugin name and description if not provided
- Create all required files in the correct locations
- Follow the directory structure below
- Register the plugin in the marketplace configuration

## Directory Structure

```text
plugins/[plugin-name]/
├── .claude-plugin/
│   └── plugin.json
└── skills/
    └── [skill-name]/
        └── SKILL.md
```

## Required Files

### 1. Plugin Manifest

Create `plugins/[plugin-name]/.claude-plugin/plugin.json`:

```json
{
  "name": "[plugin-name]",
  "description": "[description]",
  "version": "1.0.0",
  "author": { "name": "eliaslecomte" }
}
```

### 2. Marketplace Registration

Add an entry to `.claude-plugin/marketplace.json` in the `plugins` array:

```json
{
  "name": "[plugin-name]",
  "source": "./plugins/[plugin-name]",
  "description": "[description]",
  "version": "1.0.0",
  "author": { "name": "eliaslecomte" },
  "category": "productivity"
}
```

### 3. Skill Files

Create skills in `plugins/[plugin-name]/skills/[skill-name]/SKILL.md` with this structure:

```markdown
---
name: skill-name
description: What the skill does and when Claude should use it.
---

# Skill title

Instructions for the skill.

## Guidelines

- Rule 1
- Rule 2

## Format

Expected output format if applicable.
```

## Steps

1. Confirm plugin name and description with the user
2. Create the plugin directory structure
3. Create the plugin.json manifest
4. Add at least one skill
5. Register in marketplace.json
6. Add any required permissions to settings.json if skills need bash access

## Rules

- Plugin names should be lowercase with hyphens (kebab-case)
- Each plugin should have at least one skill
- Skills are organized in subdirectories with SKILL.md files
- Keep descriptions concise but informative
