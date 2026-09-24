# LoungeMC

LoungeMC was a gaming and developer community built around operating, extending, and automating multiplayer infrastructure.

The project evolved beyond simply running Minecraft servers into a practical software-engineering environment spanning **Java, Go, PHP, web development, Linux infrastructure, CI/CD, access control, monitoring, backups, and game-server orchestration**.

Much of the software here was created to solve operational problems encountered while running live community infrastructure and was released publicly where it could be useful to others.

## Projects

### CastleGuard

[CastleGuard](https://github.com/LoungeMC/CastleGuard) is an open-source permission-based access-control system for Minecraft servers.

Instead of maintaining a separate static whitelist, CastleGuard integrates with the server's existing permission system to dynamically determine whether a player should be granted access.

**Technology**
- Java
- OpenJDK 17+
- Gradle
- Spigot / Minecraft server APIs
- Permission-based access control
- TeamCity CI/CD

**Engineering focus**
- Lightweight authorization without an additional database
- Integration with existing permission providers
- Automated build and deployment workflows
- Low-maintenance access management for live communities

---

### Azuriom Status Page

[azuriom-statuspage](https://github.com/LoungeMC/azuriom-statuspage) is an Azuriom plugin developed to provide centralized, public service-status visibility for Minecraft infrastructure.

The plugin queries game servers and exposes their availability through an Azuriom-hosted status page.

**Technology**
- PHP
- Azuriom
- Laravel-style application architecture
- Database migrations
- Cron-based monitoring
- Socket/network health checks
- Minecraft Query

**Engineering focus**
- Multi-server service monitoring
- Public operational-status reporting
- Integration with an existing CMS/platform
- Automated scheduled health checks

---

### Pelican Wings Tweaked

[pelican-wings-tweaked](https://github.com/LoungeMC/pelican-wings-tweaked) contains modifications to the Go-based Wings daemon used by Pelican Panel.

The project grew from operational changes originally developed around Pterodactyl and later ported toward Pelican, including changes to server storage and SFTP behavior.

One patch separates the SFTP-visible data directory from the directory managed internally by the panel, enabling workflows such as versioned snapshots and integration with external backup systems.

**Technology**
- Go
- Linux
- Pelican / Wings
- Shell scripting
- Git patches
- SFTP
- BorgBackup-compatible backup workflows

**Engineering focus**
- Modifying upstream Go services
- Linux filesystem and storage architecture
- Backup and recovery workflows
- Operational automation
- Maintaining local patches against upstream software

---

### LoungeMC Website & Platform

LoungeMC also included development and operation of its community-facing website and supporting platform services.

Work across the project's lifetime included:

- Web application development
- PHP and JavaScript
- CMS customization
- Azuriom development
- API and service integrations
- Linux hosting
- Game-server infrastructure
- Deployment automation
- Monitoring and status tooling
- Backup and recovery
- Community authentication and authorization

Some historical repositories and services have since been retired or consolidated.

## Engineering Environment

LoungeMC served as a production environment for building and operating software against real community workloads.

```text
Languages
├── Java
├── Go
├── PHP
├── JavaScript
└── Shell

Application / Platform
├── Azuriom
├── Spigot
├── Pelican / Pterodactyl
├── Minecraft server APIs
└── Web applications

Infrastructure
├── Linux
├── SFTP
├── Game-server orchestration
├── Monitoring
├── Backup & recovery
└── Network services

Delivery
├── Git
├── Gradle
├── TeamCity
├── Automated builds
└── Deployment scripting
```

## Why LoungeMC Existed

LoungeMC was built around a simple principle:

> If an operational problem can be reliably solved in software, automate it.

That meant treating a gaming community much like any other live service: reducing manual administration, building reusable tooling, improving observability, automating deployment, and designing systems that were easier to operate and recover.

The result was a mix of **software engineering, platform engineering, DevOps, and reliability engineering** applied to a real-world community platform.

## Project Status

The original LoungeMC community is no longer under active development.

Repositories remain available where appropriate as examples, references, or open-source projects. Individual repositories may have their own maintenance status and licensing terms.

## License

Licensing varies by repository. See each project's `LICENSE` file for details.
