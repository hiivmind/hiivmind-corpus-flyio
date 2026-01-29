# CLAUDE.md

This file provides guidance to Claude Code when working with this repository.

## Overview

This is a **data-only documentation corpus** for Fly.io. It contains indexed documentation that can be queried via the `hiivmind-corpus` plugin.

**Important:** This is NOT a Claude Code plugin. Navigation and all operations are provided by the `hiivmind-corpus` plugin.

## How to Use This Corpus

### Registration

Register this corpus with your project using `hiivmind-corpus`:

```
/hiivmind-corpus register github:hiivmind/hiivmind-corpus-flyio
```

This adds an entry to `.hiivmind/corpus/registry.yaml` in your project.

### Navigation

Once registered, ask questions about Fly.io and the navigate skill will find relevant documentation:

```
How do I deploy a Python app to Fly.io?
What's the difference between Machines and Apps?
```

Or explicitly navigate:

```
/hiivmind-corpus navigate flyio "postgres configuration"
```

## Directory Structure

```
hiivmind-corpus-flyio/
├── config.yaml          # Source definitions and keywords
├── index.md             # Main documentation index
├── index-*.md           # Sub-indexes for tiered sections
├── uploads/             # Local document uploads
├── .source/             # Cloned git sources (gitignored)
├── .cache/              # Cached web content (gitignored)
└── README.md
```

## Key Files

| File | Purpose | Editable? |
|------|---------|-----------|
| `config.yaml` | Source definitions, keywords, commit tracking | Via `hiivmind-corpus-refresh` |
| `index.md` | Main documentation index with summaries | Via `hiivmind-corpus-build/enhance/refresh` |
| `index-*.md` | Sub-indexes for large sections | Via `hiivmind-corpus-build/enhance/refresh` |

## Maintenance

This corpus is maintained using `hiivmind-corpus` skills:

| Skill | Purpose |
|-------|---------|
| `hiivmind-corpus-build` | Build/rebuild the documentation index |
| `hiivmind-corpus-refresh` | Update index from upstream changes |
| `hiivmind-corpus-enhance` | Deepen coverage on specific topics |
| `hiivmind-corpus-add-source` | Add new documentation sources |

### Example Commands

```
# Refresh from upstream
/hiivmind-corpus refresh flyio

# Enhance a topic
/hiivmind-corpus enhance flyio authentication

# Add another source
/hiivmind-corpus add-source flyio https://github.com/fly-apps/example
```

## Corpus Routing

This corpus auto-triggers for questions containing these keywords (defined in `config.yaml`):

- flyio, fly.io, fly
- deployment, hosting, edge, cloud

## Requirements

- `hiivmind-corpus` plugin installed (provides all operations)
- Git (for source cloning and updates)
