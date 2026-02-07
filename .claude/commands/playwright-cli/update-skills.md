# Update Playwright CLI skills from upstream

Fetch the latest Playwright CLI skill files from the official repository and update the local copies.

## Source

Repository: `microsoft/playwright-cli`
Branch: `main`
Base URL: `https://raw.githubusercontent.com/microsoft/playwright-cli/main/skills/playwright-cli`

## Files to sync

| Remote path | Local path |
| ----------- | ---------- |
| `SKILL.md` | `plugins/web/skills/playwright-cli/SKILL.md` |
| `references/request-mocking.md` | `plugins/web/skills/playwright-cli/references/request-mocking.md` |
| `references/running-code.md` | `plugins/web/skills/playwright-cli/references/running-code.md` |
| `references/session-management.md` | `plugins/web/skills/playwright-cli/references/session-management.md` |
| `references/storage-state.md` | `plugins/web/skills/playwright-cli/references/storage-state.md` |
| `references/test-generation.md` | `plugins/web/skills/playwright-cli/references/test-generation.md` |
| `references/tracing.md` | `plugins/web/skills/playwright-cli/references/tracing.md` |
| `references/video-recording.md` | `plugins/web/skills/playwright-cli/references/video-recording.md` |

## Steps

1. For each file in the table above, fetch the raw content from the base URL
2. Compare with the existing local file
3. If the content differs, overwrite the local file with the fetched content
4. If new files exist upstream that are not in the table, create them locally

## Rules

- Always fetch from the `main` branch
- Report a summary of changes: which files were updated, added, or unchanged
- Do not modify fetched content — copy it verbatim
- If a fetch fails, report the error and continue with remaining files
