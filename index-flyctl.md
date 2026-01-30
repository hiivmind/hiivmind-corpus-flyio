# flyctl CLI Reference - Navigation Guide

> Part of the Fly.io Documentation Corpus
> Back to [main index](index.md)

---

## ⚡ Important: Using This Reference

The flyctl command reference contains **329 auto-generated files**. Instead of listing them all here, use **Grep** to search efficiently:

### Search for a Specific Command

```bash
# Find a specific command (e.g., "fly deploy")
grep -l "fly deploy" .source/flyio/flyctl/cmd/*.md

# Read the deploy command documentation
grep -n "^## fly deploy" .source/flyio/flyctl/cmd/fly_deploy.md -A 50
```

### Search by Keyword

```bash
# Find all commands related to "scale"
grep -l "scale" .source/flyio/flyctl/cmd/*.md

# Find commands for "postgres"
grep -l "postgres" .source/flyio/flyctl/cmd/*.md
```

---

## Quick Reference - Most Common Commands

### App Management
- **fly deploy** `flyio:flyctl/cmd/fly_deploy.md` ⚡ GREP - Deploy your application
- **fly launch** `flyio:flyctl/cmd/fly_launch.md` ⚡ GREP - Create and launch a new app
- **fly apps list** `flyio:flyctl/cmd/fly_apps_list.md` ⚡ GREP - List all apps
- **fly apps create** `flyio:flyctl/cmd/fly_apps_create.md` ⚡ GREP - Create a new app
- **fly apps destroy** `flyio:flyctl/cmd/fly_apps_destroy.md` ⚡ GREP - Delete an app
- **fly status** `flyio:flyctl/cmd/fly_status.md` ⚡ GREP - Show app status

### Scaling
- **fly scale count** `flyio:flyctl/cmd/fly_scale_count.md` ⚡ GREP - Scale number of instances
- **fly scale vm** `flyio:flyctl/cmd/fly_scale_vm.md` ⚡ GREP - Scale VM size (CPU/RAM)
- **fly scale memory** `flyio:flyctl/cmd/fly_scale_memory.md` ⚡ GREP - Set memory allocation

### Secrets
- **fly secrets list** `flyio:flyctl/cmd/fly_secrets_list.md` ⚡ GREP - List app secrets
- **fly secrets set** `flyio:flyctl/cmd/fly_secrets_set.md` ⚡ GREP - Set secrets
- **fly secrets unset** `flyio:flyctl/cmd/fly_secrets_unset.md` ⚡ GREP - Remove secrets

### Logs & Monitoring
- **fly logs** `flyio:flyctl/cmd/fly_logs.md` ⚡ GREP - View application logs
- **fly doctor** `flyio:flyctl/cmd/fly_doctor.md` ⚡ GREP - Diagnose common issues
- **fly checks list** `flyio:flyctl/cmd/fly_checks_list.md` ⚡ GREP - View health checks

### Machines
- **fly machine run** `flyio:flyctl/cmd/fly_machine_run.md` ⚡ GREP - Create and start a Machine
- **fly machine list** `flyio:flyctl/cmd/fly_machine_list.md` ⚡ GREP - List Machines
- **fly machine stop** `flyio:flyctl/cmd/fly_machine_stop.md` ⚡ GREP - Stop a Machine
- **fly machine destroy** `flyio:flyctl/cmd/fly_machine_destroy.md` ⚡ GREP - Remove a Machine

### Postgres
- **fly postgres create** `flyio:flyctl/cmd/fly_postgres_create.md` ⚡ GREP - Create Postgres cluster
- **fly postgres attach** `flyio:flyctl/cmd/fly_postgres_attach.md` ⚡ GREP - Connect app to Postgres
- **fly postgres connect** `flyio:flyctl/cmd/fly_postgres_connect.md` ⚡ GREP - Open psql console
- **fly postgres db** `flyio:flyctl/cmd/fly_postgres_db.md` ⚡ GREP - Manage databases

### Managed Postgres (MPG)
- **fly mpg** `flyio:flyctl/cmd/fly_mpg.md` ⚡ GREP - Manage Managed Postgres clusters
- **fly mpg detach** `flyio:flyctl/cmd/fly_mpg_detach.md` ⚡ GREP - Detach managed Postgres cluster from an app

### Volumes
- **fly volumes create** `flyio:flyctl/cmd/fly_volumes_create.md` ⚡ GREP - Create a volume
- **fly volumes list** `flyio:flyctl/cmd/fly_volumes_list.md` ⚡ GREP - List volumes
- **fly volumes delete** `flyio:flyctl/cmd/fly_volumes_delete.md` ⚡ GREP - Remove a volume

### SSH & Console
- **fly ssh console** `flyio:flyctl/cmd/fly_ssh_console.md` ⚡ GREP - Open SSH console
- **fly ssh sftp** `flyio:flyctl/cmd/fly_ssh_sftp.md` ⚡ GREP - SFTP file transfer

---

## Command Categories

### Installation & Setup
**Path:** `flyio:flyctl/install.html.markerb`

Installation guide for macOS, Linux, and Windows.

### Core App Commands
- `fly apps` - App management
- `fly launch` - Create and deploy
- `fly deploy` - Deploy changes
- `fly status` - App status

### Scaling & Resources
- `fly scale` - Scale instances and resources
- `fly regions` - Manage deployment regions
- `fly vm` - VM size management

### Configuration
- `fly config` - View and manage config
- `fly secrets` - Secret management
- `fly env` - Environment variables

### Monitoring & Debugging
- `fly logs` - View logs
- `fly doctor` - Diagnose issues
- `fly checks` - Health checks
- `fly monitor` - Real-time monitoring

### Database Commands
- `fly postgres` - Managed Postgres
- `fly redis` - Redis commands
- `fly volumes` - Volume management

### Networking
- `fly ips` - IP address management
- `fly certs` - TLS certificate management
- `fly proxy` - Local proxy to apps

### Machine Management
- `fly machine` - Direct Machine control
- `fly machine run` - Create Machines
- `fly machine update` - Modify Machines

### Authentication & Org
- `fly auth` - Login and authentication
- `fly orgs` - Organization management
- `fly tokens` - API token management

---

## Finding Commands

**By task:**
```bash
# What commands help with deployment?
grep -l "deploy" .source/flyio/flyctl/cmd/*.md

# What commands manage databases?
grep -l "database\|postgres\|db" .source/flyio/flyctl/cmd/*.md
```

**By resource:**
```bash
# All Machine commands
ls .source/flyio/flyctl/cmd/fly_machine*.md

# All Postgres commands
ls .source/flyio/flyctl/cmd/fly_postgres*.md

# All Volume commands
ls .source/flyio/flyctl/cmd/fly_volume*.md
```
