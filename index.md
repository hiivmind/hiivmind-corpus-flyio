# Fly.io Documentation Corpus

> 748 documentation files organized by topic
> Last updated: 2026-01-30

## How to Use This Index

This corpus uses a **tiered index** due to its size. Start here for an overview and quick lookups, then drill into sub-indexes for detailed entries.

---

## Quick Reference

Common lookups (full path for direct access):

- **Install flyctl** `flyio:flyctl/install.html.markerb` - Install the Fly.io CLI on your system
- **Launch an app** `flyio:getting-started/launch.html.markerb` - Quickstart guide to deploy your first app
- **Deploy with fly deploy** `flyio:flyctl/cmd/fly_deploy.md` - Deploy app changes to Fly.io
- **Scale an app** `flyio:flyctl/cmd/fly_scale.md` - Scale app resources and regions
- **Create Postgres** `flyio:postgres/getting-started/create-pg-cluster.html.md` - Set up managed Postgres database
- **Machines API** `flyio:machines/api/machines-resource.html.md` - REST API for Fly Machines
- **Networking basics** `flyio:networking/private-networking.html.md` - Private networks and service discovery
- **Secrets management** `flyio:apps/secrets.html.markerb` - Store and use application secrets
- **View logs** `flyio:flyctl/cmd/fly_logs.md` - Access application logs
- **Troubleshooting** `flyio:getting-started/troubleshooting.html.md` - Common issues and solutions

---

## Getting Started
*First steps with Fly.io - installation, signup, and deploying your first app*

→ See [index-getting-started.md](index-getting-started.md) for 7 detailed entries

Key topics: flyctl installation, account setup, fly launch, framework-specific guides, troubleshooting

---

## Apps
*Application deployment, configuration, and management on Fly.io*

→ See [index-apps.md](index-apps.md) for 14 detailed entries

Key topics: App lifecycle, secrets, scaling, availability, production readiness, build configuration

---

## Fly Machines
*Low-level VM control with the Machines REST API*

→ See [index-machines.md](index-machines.md) for 22 detailed entries

Key topics: Machines API, VM lifecycle, runtime environment, guides & examples, flyctl for Machines

---

## Databases & Storage
*Managed Postgres, volumes, and database integrations*

→ See [index-databases.md](index-databases.md) for ~60 detailed entries

Key topics: Managed Postgres, Postgres extensions, high availability, volumes, Redis (Upstash), LiteFS

---

## Networking
*Private networks, load balancing, certificates, and service discovery*

→ See [index-networking.md](index-networking.md) for 14 detailed entries

Key topics: Private networking, public networking, load balancing, TLS certificates, custom domains

---

## flyctl CLI Reference
*Complete command reference for the Fly.io CLI (329 commands)*

→ See [index-flyctl.md](index-flyctl.md) for navigation guide

⚡ Most flyctl commands are auto-generated reference docs. Use Grep to search:
```bash
grep -n "^## fly {command}" .source/flyio/flyctl/cmd/ -A 20
```

Key command categories: apps, machines, postgres, volumes, scale, deploy, logs, secrets

---

## Languages & Frameworks
*Framework-specific deployment guides and examples*

→ See [index-languages.md](index-languages.md) for ~80 detailed entries

Key topics: Rails, Django, Elixir/Phoenix, JavaScript/Node, Python, Rust, Laravel

---

## Reference & Platform
*Platform architecture, configuration reference, and advanced topics*

→ See [index-reference.md](index-reference.md) for ~50 detailed entries

Key topics: fly.toml configuration, regions, pricing, security, GPUs, MCP, monitoring, blueprints
