# Update Vercel agent skills from upstream

Fetch the latest skill files from the Vercel agent-skills repository and update the local copies across all plugins.

## Source

Repository: `vercel-labs/agent-skills`
Branch: `main`
Base URL: `https://raw.githubusercontent.com/vercel-labs/agent-skills/main/skills`

## Files to sync

### react plugin

| Remote path | Local path |
| ----------- | ---------- |
| `react-best-practices/SKILL.md` | `plugins/react/skills/react-best-practices/SKILL.md` |
| `react-best-practices/AGENTS.md` | `plugins/react/skills/react-best-practices/AGENTS.md` |
| `composition-patterns/SKILL.md` | `plugins/react/skills/composition-patterns/SKILL.md` |
| `composition-patterns/AGENTS.md` | `plugins/react/skills/composition-patterns/AGENTS.md` |

### react-native plugin

| Remote path | Local path |
| ----------- | ---------- |
| `react-native-skills/SKILL.md` | `plugins/react-native/skills/react-native-skills/SKILL.md` |
| `react-native-skills/AGENTS.md` | `plugins/react-native/skills/react-native-skills/AGENTS.md` |

### web plugin

| Remote path | Local path |
| ----------- | ---------- |
| `web-design-guidelines/SKILL.md` | `plugins/web/skills/web-design-guidelines/SKILL.md` |

## Steps

1. For each file in the tables above, fetch the raw content from the base URL
2. Compare with the existing local file
3. If the content differs, overwrite the local file with the fetched content
4. If new files exist upstream that are not in the tables, create them locally

## Rules

- Always fetch from the `main` branch
- Report a summary of changes per plugin: which files were updated, added, or unchanged
- Do not modify fetched content — copy it verbatim
- If a fetch fails, report the error and continue with remaining files
