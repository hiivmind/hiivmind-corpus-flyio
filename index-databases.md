# Databases & Storage - Detailed Index

> Part of the Fly.io Documentation Corpus
> Back to [main index](index.md)

---

## Managed Postgres

### Getting Started
- **Postgres index** `flyio:postgres/index.html.md` - Main Postgres documentation
- **Getting started** `flyio:postgres/getting-started.html.markerb` - Postgres quickstart overview
- **Create a cluster** `flyio:postgres/getting-started/create-pg-cluster.html.md` - Set up your first Postgres database
- **What you should know** `flyio:postgres/getting-started/what-you-should-know.html.md` - Important concepts before deploying Postgres

### Connecting
- **Connecting overview** `flyio:postgres/connecting.html.md` - Connection methods and patterns
- **Connect to Postgres** `flyio:postgres/connecting/connecting-internal.html.md` - Internal app connections
- **Connect from outside Fly** `flyio:postgres/connecting/connecting-external.html.md` - External database access

### Managing
- **Managing overview** `flyio:postgres/managing.html.markerb` - Database management tasks
- **Scale Postgres** `flyio:postgres/managing/scaling.html.md` - Vertical and horizontal scaling
- **High availability** `flyio:postgres/managing/high-availability.html.md` - HA setup and failover
- **Backup and restore** `flyio:postgres/managing/backup-and-restore.html.md` - Database backup strategies
- **Monitoring** `flyio:postgres/managing/monitoring.html.md` - Monitor database health and performance

### Advanced
- **Advanced guides** `flyio:postgres/managing.html.markerb` - Advanced Postgres topics

---

## Volumes

- **Volumes index** `flyio:volumes/index.html.markerb` - Main volumes documentation
- **Volumes overview** `flyio:volumes/overview.html.markerb` - What are Fly Volumes and when to use them
- **Manage volumes** `flyio:volumes/volume-manage.html.markerb` - Create, resize, and delete volumes
- **Volume snapshots** `flyio:volumes/snapshots.html.markerb` - Backup and restore volumes
- **Volume states** `flyio:volumes/volume-states.html.markerb` - Volume lifecycle and states

---

## LiteFS (Distributed SQLite)

### Getting Started
- **LiteFS index** `flyio:litefs/index.html.markerb` - Main LiteFS documentation
- **How it works** `flyio:litefs/how-it-works.html.markerb` - LiteFS architecture and replication
- **Speedrun** `flyio:litefs/speedrun.html.markerb` - Quick LiteFS setup
- **Getting started with Fly.io** `flyio:litefs/getting-started-fly.html.markerb` - Deploy LiteFS on Fly
- **Getting started with Docker** `flyio:litefs/getting-started-docker.html.markerb` - Use LiteFS locally

### Configuration & Operations
- **Configuration** `flyio:litefs/config.html.markerb` - LiteFS config file reference
- **Primary election** `flyio:litefs/primary.html.markerb` - How primary node is selected
- **Events** `flyio:litefs/events.html.markerb` - LiteFS event system
- **Mount** `flyio:litefs/mount.html.markerb` - Mounting LiteFS filesystems
- **Run** `flyio:litefs/run.html.markerb` - Running LiteFS processes
- **Proxy** `flyio:litefs/proxy.html.markerb` - HTTP proxy for read/write routing

### Backup & Recovery
- **Backup** `flyio:litefs/backup.html.markerb` - Local backup strategies
- **Cloud backups** `flyio:litefs/cloud-backups.html.markerb` - S3-compatible cloud backups
- **Cloud restore** `flyio:litefs/cloud-restore.html.markerb` - Restore from cloud backups
- **Disaster recovery** `flyio:litefs/disaster-recovery.html.markerb` - Recovery procedures

### Data Management
- **Import** `flyio:litefs/import.html.markerb` - Import existing SQLite databases
- **Export** `flyio:litefs/export.html.markerb` - Export LiteFS databases
- **Migrations** `flyio:litefs/migrations.html.markerb` - Running schema migrations
- **Position** `flyio:litefs/position.html.markerb` - Replication position tracking

### Reference
- **FAQ** `flyio:litefs/faq.html.markerb` - Frequently asked questions
- **Releases** `flyio:litefs/releases.html.markerb` - LiteFS version history

---

## Database Integrations

- **Upstash Redis** `flyio:upstash/` - Managed Redis via Upstash
- **Supabase** `flyio:supabase/` - Supabase integration on Fly.io
- **Tigris** `flyio:tigris/` - Object storage with Tigris
