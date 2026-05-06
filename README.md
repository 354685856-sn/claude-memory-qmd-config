# Claude Memory QMD Config

QMD vector memory configuration for Claude Code context retrieval and long-term agent memory experiments.

## Why

Long-running AI agent work needs memory that is searchable, scoped, and easy to inspect. This repository keeps a small example configuration for a QMD-backed memory workflow using Markdown files as the source of truth.

## What is inside

| File | Purpose |
|------|---------|
| [memory-config.json](./memory-config.json) | QMD memory backend configuration. |
| [MEMORY.md](./MEMORY.md) | Example long-term memory file with user preferences, project knowledge, and memory settings. |

## Configuration summary

| Setting | Value |
|---------|-------|
| Backend | `qmd` |
| Search mode | hybrid vector + text |
| Max results | 10 |
| Max injected characters | 5000 |
| Update interval | 5 minutes |
| Temporal decay | enabled, 30-day half-life |
| MMR deduplication | enabled, lambda 0.7 |

## Intended workflow

1. Keep durable facts and project knowledge in Markdown.
2. Let QMD index the configured paths.
3. Retrieve relevant snippets during Claude Code sessions.
4. Cite memory sources when injected context influences an answer.
5. Periodically clean stale or low-value memory entries.

## Files currently indexed by the example config

```text
/Users/mac/bin/.claude/memory/MEMORY.md
/Users/mac/bin/.claude/memory/daily
/Users/mac/bin/.claude/work-progress.md
```

These paths are local to the original setup. Adjust them before reusing this configuration on another machine.

## Roadmap

- [ ] Add installation instructions for QMD.
- [ ] Add a minimal verification command.
- [ ] Add a portable sample config using relative paths.
- [ ] Add examples of good and bad memory entries.
- [ ] Document how this config connects to Obsidian vault notes.

## License

No license has been selected yet.
