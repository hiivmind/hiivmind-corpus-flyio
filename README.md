# Fly.io Documentation Corpus

A Claude Code plugin providing always-current access to Fly.io documentation with intelligent navigation.

## Features

- **Indexed Navigation**: Structured index of all Fly.io documentation with summaries, key concepts, and cross-references
- **Automatic Updates**: Incremental index updates from upstream documentation changes
- **Smart Matching**: Finds relevant docs based on concepts, summaries, and section headings

## Installation

### As a Plugin

```bash
# Add the marketplace containing this plugin
/plugin marketplace add hiivmind/hiivmind-corpus-flyio

# Install the plugin
/plugin install hiivmind-corpus-flyio

# Restart Claude Code
```

### Manual Installation

Clone this repository to your Claude Code plugins directory.

## First-Time Setup

After installing, use the `hiivmind-corpus-build` skill to build the index:

```
Please build the Fly.io documentation index
```

This requires the `hiivmind-corpus` meta-plugin to be installed.

## Maintenance Skills

This corpus is managed by **hiivmind-corpus** skills:

| Skill | Purpose |
|-------|---------|
| `hiivmind-corpus-add-source` | Add new documentation sources |
| `hiivmind-corpus-build` | Build/rebuild the documentation index |
| `hiivmind-corpus-enhance` | Deepen coverage on specific topics |
| `hiivmind-corpus-refresh` | Update index from upstream changes |

## Usage

### Automatic Navigation

The navigation skill is model-invoked. Simply ask questions about Fly.io:

```
How do I deploy a Python app to Fly.io?
What's the difference between Machines and Apps?
How do I set up Postgres on Fly.io?
```

Claude will automatically find and cite relevant documentation.

### Index Updates

Refresh from upstream changes (uses `hiivmind-corpus-refresh`):

```
Refresh the Fly.io corpus from upstream
```

Full rebuild (uses `hiivmind-corpus-build`):

```
Rebuild the Fly.io documentation index from scratch
```

Enhance a specific topic (uses `hiivmind-corpus-enhance`):

```
Add more detail about authentication to the Fly.io index
```

## Skills

### hiivmind-corpus-navigate-flyio

Finds relevant documentation for Fly.io-related coding tasks. Automatically invoked when you ask about:

- Deployment and hosting
- Machines and apps
- Databases (Postgres, Redis, etc.)
- Networking and load balancing
- Edge computing
- flyctl CLI commands

## File Structure

```
hiivmind-corpus-flyio/
├── .claude-plugin/
│   └── plugin.json           # Plugin manifest
├── commands/
│   └── navigate.md           # Documentation navigation
├── data/
│   ├── config.yaml           # Source repo + settings
│   └── index.md              # Generated documentation index
├── .source/                  # Cloned docs repo (gitignored)
└── README.md
```

## Configuration

The `data/config.yaml` and `data/index.md` files are managed by hiivmind-corpus skills. Do not edit them manually.

To add new sources, use `hiivmind-corpus-add-source`. To rebuild or enhance the index, use `hiivmind-corpus-build` or `hiivmind-corpus-enhance`.

## Requirements

- `hiivmind-corpus` meta-plugin installed (provides maintenance skills)
- Git (for cloning and updating documentation)
- Claude Code with plugin support

## License

MIT
