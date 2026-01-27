# Fly.io Documentation Corpus

A data-only documentation corpus for Fly.io. Use with the `hiivmind-corpus` plugin for navigation and maintenance.

## What is This?

This repository contains:
- **Indexed documentation** - Structured index of Fly.io docs with summaries and cross-references
- **Source tracking** - Configuration tracking upstream documentation commits
- **Keywords** - Routing keywords for automatic corpus selection

This is NOT a Claude Code plugin. All operations (navigation, building, refreshing) are provided by the `hiivmind-corpus` plugin.

## Quick Start

### 1. Install the hiivmind-corpus plugin

```bash
# In Claude Code
/plugin install hiivmind/hiivmind-corpus
```

### 2. Register this corpus

```bash
# Register from GitHub
/hiivmind-corpus register github:hiivmind/hiivmind-corpus-flyio
```

### 3. Start asking questions

```
How do I deploy a Rails app to Fly.io?
What are Fly Machines?
How do I configure Postgres on Fly.io?
```

## File Structure

```
hiivmind-corpus-flyio/
├── config.yaml          # Source definitions, keywords, tracking
├── index.md             # Main documentation index
├── index-apps.md        # Apps section index
├── index-databases.md   # Databases section index
├── index-flyctl.md      # CLI reference index
├── index-getting-started.md
├── index-languages.md   # Framework guides index
├── index-machines.md    # Machines section index
├── index-networking.md  # Networking section index
├── index-reference.md   # Reference docs index
├── uploads/             # Local document uploads
├── .source/             # Cloned docs (gitignored)
├── .cache/              # Web cache (gitignored)
└── README.md
```

## Maintenance

Use `hiivmind-corpus` skills to maintain this corpus:

| Command | Purpose |
|---------|---------|
| `/hiivmind-corpus refresh flyio` | Update from upstream changes |
| `/hiivmind-corpus enhance flyio <topic>` | Add depth to a topic |
| `/hiivmind-corpus build flyio` | Full rebuild |
| `/hiivmind-corpus add-source flyio <url>` | Add new source |

## config.yaml Schema

```yaml
schema_version: 2

corpus:
  name: "flyio"
  display_name: "Fly.io"
  keywords:            # For automatic routing
    - flyio
    - fly.io
    - deployment

sources:
  - id: flyio
    type: git
    repo_url: https://github.com/superfly/docs
    branch: main
    last_commit_sha: "..."
    last_indexed_at: "..."
```

## Requirements

- `hiivmind-corpus` plugin (provides all operations)
- Git (for source management)

## License

MIT
