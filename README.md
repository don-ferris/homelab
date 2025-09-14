# HomeLab - Purpose & Goals

## PURPOSE
The purpose of my homelab, a collection of hardware and software, is to provide online and digital services that make my digital life rich, robust, and convenient while also protecting the privacy and confidentiality of my personal data through self-hosting.

## GOALS
- Run services that improve my daily life — such as media servers, home automation, personal financial and project management, websites, and much more.
- Make everything as private and secure as possible, by keeping my data under my control.
- Reduce (eliminate, if possible) my dependence on cloud services (Google, Dropbox, etc.) for sensitive files and data.
- Build systems that are fun to use, reliable during power or internet outages, and easy to upgrade over time.
- Learn and experiment with new technology at my own pace.
  
# Homelab (This) Meta Project Plan - Purpose & Goals

## PURPOSE
This meta project plan is an overview for the many projects that will collectively result in my homelab. In particular, this plan will focus on infrastructure, standards, procedures, and methods for making sure these services are stable and highly reliable, well documented, and able to be quickly recovered if something goes wrong.

## GOALS
- Organize all my current and future homelab projects in one easy-to-find place.
- Define clear standards, procedures, and repeatable steps for deploying, upgrading, and maintaining every part of the homelab.
- Write clear documentation as I go, so I can always remember what was done and how it works.
- Mandate careful documentation for every service, configuration, and custom script using README files and a centralized wiki.
- Set up simple, reliable backup routines for all important files and configurations, with step-by-step instructions for recovery.
- Start every project with strong security basics, specifying baseline security practices for every new deployment, including safe remote access and restricted permissions.
- Continually track, review, and improve my setup as my needs or hardware change.
- Maintain a single, organized place (this plan) for tracking homelab projects, pending ideas, and ongoing improvements.

## WILLWIF: What It Looks Like When It’s Finished

### User Experience

When my homelab is complete, I interact with all my services through a Flame dashboard as my central hub, accessible from any trusted device. All my daily routines—listening to music, watching movies, downloading media, updating finances, checking home automation status, managing projects, monitoring backup status, and editing Office documents—are easily accessible, organized, and streamlined from this dashboard. Every key action or service is just a click away.

***

### Reliability and Recovery

All services are constantly monitored by automatic, scheduled tests. Any issue triggers an immediate push notification that includes a direct link to a clear dashboard and to the tools needed for recovery. Recovery from failures is as fast and easy as possible—ideally with a single command or script. Every script includes built-in help instructions that appear when run with --help. Detailed documentation ensures that even rarely-used recovery processes are just as simple—step-by-step guidance is always available, both in scripts and in README files.

***

### Security and Privacy

Every piece of my homelab is locked down according to its role:
- SSH access uses secure keys only, with password login disabled.
- Externally-exposed services use Cloudflare tunnels for secure remote access. Eventually, Cloudflare “apps”—accessible only on specified trusted devices—will be used for even tighter security.
- Services use strong, random, unique passwords managed by Bitwarden, and some critical systems (reverse proxies, key services) include Multi-Factor Authentication (MFA)—most likely using Authentik or Authelia, depending on the needs and connections of each service.
- Security notifications only appear for real, persistent threats or confirmed intrusions—no noisy alerts.
- Where my most private/confidential data lives, access is protected with a bastion host and backups are stored in a way that makes them “immutable”: the backup system is offline except when actively backing up, with detailed restore procedures documented and tested.

***

### Documentation

Every project and service includes its own README.md, built on a standardized template. All user data (databases, config files, and anything that changes during use) is stored within a dedicated ./data directory. Automated GitHub syncing means that both configurations and user data are backed up on schedule with version control.
Documentation for each project includes:
- Basic project info in the homelab wiki (Dokuwiki), including credentials, installation guides, restore-from-backup instructions, and links to the official docs, GitHub repos, and community support.
- Step-by-step beginner instructions and technical notes for advanced users (“power scripts” display their README and help via a --help command).
- Disaster recovery and restore steps, always visible within both the wiki and the related GitHub repos.

***

### Services

#### Always-On (VPS)

The following core services are always running, fully documented, and have regular tested backups:
- Dokuwiki (documentation)
- Flame Dashboard (main UI)
- Document service (cloud storage and office alternatives)
- NotesNook (for notes)
- Calendar (Baikal)
- Netbird (secure network)
- Nginx Proxy Manager
- Authentik/Authelia (authentication/MFA)
- Portainer (container management)
- Watchtower (auto updates)
- Autoheal (container recovery)
- Uptime Kuma (monitoring)
- LinkAce or Karakeep (bookmarks)
- Actual Budget (finances)
- Lychee (photos)
- All personal websites/blogs

#### On Unless Disabled/Outage (BoraBora/local)

These services are always running unless shut down for power savings/outages, with complete documentation and backup/restore:
- Jellyfin (media server)
- Home Assistant (automation/hub)
- OpenWebUI + Ollama for local AI/LLM (primarily used by Home Assistant but also for general household use/information
- Audiobookshelf/Libation (audiobooks)
- Kavita or Calibre + Readarr (ebooks, comics)
- Sonarr/Radarr/Lidarr/Overseerr (media management)
- Nzbget (downloads)
- Paperless (scanned documents)
- NFS/SMB network storage connectors
- Watchtower, Autoheal, Uptime Kuma, Portainer (for local containers and monitoring)
