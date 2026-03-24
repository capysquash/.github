<div align="center">
  
 

  # CAPYSQUASH

  **The modern platform for Postgres migration cleanup.**

  [![Engine](https://img.shields.io/badge/engine-pgsquash--engine-4169E1?style=flat-square&logo=postgresql&logoColor=white)](https://github.com/CAPYSQUASH/pgsquash-engine)
  [![Studio](https://img.shields.io/badge/studio-typescript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://github.com/CAPYSQUASH/capysquash-studio)
  [![VS Code](https://img.shields.io/badge/vscode-extension-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)](https://github.com/CAPYSQUASH/capysquash-vscode)
  [![Docs](https://img.shields.io/badge/docs-fumadocs-0EA5E9?style=flat-square)](https://github.com/CAPYSQUASH/capysquash-docs)

 [![Website](https://img.shields.io/badge/Website-capysquash.dev-0F172A?style=for-the-badge)](https://capysquash.dev)
  [![Platform](https://img.shields.io/badge/platform-next.js-000000?style=for-the-badge&logo=nextdotjs)](https://github.com/CAPYSQUASH/capysquash-platform)
  [![CLI](https://img.shields.io/badge/cli-go-00ADD8?style=for-the-badge&logo=go)](https://github.com/CAPYSQUASH/capysquash-cli)
  [![API](https://img.shields.io/badge/api-go-00ADD8?style=for-the-badge&logo=go)](https://github.com/CAPYSQUASH/capysquash-api)
</div>

---

## Overview

**CapySquash** turns migration sprawl into clean, reviewable, deployable SQL history.

Built for indie hackers, startup teams, and fast-moving product devs who want to ship database changes with less risk and less ceremony.

**Why teams use it:**
- Keep migration history lean and maintainable
- Catch risky changes before they reach production
- Use the same core behavior across platform, CLI, API, and editor tooling

## Key capabilities

<table>
<tr>
<td width="50%">

### Platform experience
- One-click cleanup workflows
- Project-level visibility and orchestration
- Team-friendly operational surface

### Developer velocity
- Terminal-first CLI for power users
- API-first integration for automation
- VS Code and studio surfaces for day-to-day flow

</td>
<td width="50%">

### Safety and confidence
- Parser-grade migration analysis
- Risk-aware validation before apply
- Consistent behavior from local to CI to production

### Ecosystem alignment
- Shared engine across products
- Cohesive docs and workflows
- No duplicated logic across surfaces

</td>
</tr>
</table>

## Tech stack

<div align="center">

| Technology | Role |
|---|---|
| ![Next.js](https://img.shields.io/badge/Next.js-Platform-000000?style=for-the-badge&logo=nextdotjs) | Platform application |
| ![Go](https://img.shields.io/badge/Go-Engine%20%2B%20API-00ADD8?style=for-the-badge&logo=go&logoColor=white) | CLI, API, and core execution |
| ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Core-4169E1?style=for-the-badge&logo=postgresql&logoColor=white) | Migration and schema domain |
| ![TypeScript](https://img.shields.io/badge/TypeScript-UI%20Surfaces-3178C6?style=for-the-badge&logo=typescript&logoColor=white) | Studio, VS Code, and frontend surfaces |

</div>

## Ecosystem map

### Main product

| Repository | Purpose |
|---|---|
| [`capysquash-platform`](https://github.com/CAPYSQUASH/capysquash-platform) | The main product: one-click cleanup, orchestration, and team workflows |

### Supporting tools

| Repository | Purpose |
|---|---|
| [`capysquash-cli`](https://github.com/CAPYSQUASH/capysquash-cli) | Terminal-first workflow for power users and CI |
| [`capysquash-api`](https://github.com/CAPYSQUASH/capysquash-api) | REST layer for integrations, automation, and services |
| [`capysquash-studio`](https://github.com/CAPYSQUASH/capysquash-studio) | Web management interface for operational workflows |
| [`capysquash-vscode`](https://github.com/CAPYSQUASH/capysquash-vscode) | In-editor workflow support for VS Code users |

### Core technology + docs

| Repository | Purpose |
|---|---|
| [`pgsquash-engine`](https://github.com/CAPYSQUASH/pgsquash-engine) | Core migration intelligence used by CLI/API/platform surfaces |
| [`capysquash-docs`](https://github.com/CAPYSQUASH/capysquash-docs) | Product docs, technical docs, and ecosystem guides |
| [`homebrew-tap`](https://github.com/CAPYSQUASH/homebrew-tap) | Homebrew distribution for CLI installation |

### Adjacent work

| Repository | Purpose |
|---|---|
| [`capydb`](https://github.com/CAPYSQUASH/capydb) | Framework-native Postgres initiative adjacent to the ecosystem |

## Quick flow

<table>
<tr>
<td align="center" width="25%">
<img src="https://api.iconify.design/lucide:folder-git-2.svg?color=%23f97316" width="44" /><br/>
<strong>1. Connect</strong><br/>
Bring your migration history
</td>
<td align="center" width="25%">
<img src="https://api.iconify.design/lucide:scan-search.svg?color=%23f97316" width="44" /><br/>
<strong>2. Analyze</strong><br/>
Detect drift and risky patterns
</td>
<td align="center" width="25%">
<img src="https://api.iconify.design/lucide:layers-2.svg?color=%23f97316" width="44" /><br/>
<strong>3. Squash</strong><br/>
Consolidate into cleaner SQL
</td>
<td align="center" width="25%">
<img src="https://api.iconify.design/lucide:rocket.svg?color=%23f97316" width="44" /><br/>
<strong>4. Ship</strong><br/>
Deploy with confidence
</td>
</tr>
</table>

## Where to start

| If you want to... | Start here |
|---|---|
| Use the main product experience | [`capysquash-platform`](https://github.com/CAPYSQUASH/capysquash-platform) |
| Work from terminal/CI | [`capysquash-cli/GETTING_STARTED.md`](https://github.com/CAPYSQUASH/capysquash-cli/blob/main/GETTING_STARTED.md) |
| Integrate over HTTP | [`capysquash-api/README.md`](https://github.com/CAPYSQUASH/capysquash-api/blob/main/README.md) |
| Explore full documentation | [`capysquash-docs`](https://github.com/CAPYSQUASH/capysquash-docs) |

## Documentation

<div align="center">

| Resource | Link |
|---|---|
| Platform docs | [capysquash-platform/README.md](https://github.com/CAPYSQUASH/capysquash-platform/blob/main/README.md) |
| CLI getting started | [capysquash-cli/GETTING_STARTED.md](https://github.com/CAPYSQUASH/capysquash-cli/blob/main/GETTING_STARTED.md) |
| API docs | [capysquash-api/docs](https://github.com/CAPYSQUASH/capysquash-api/tree/main/docs) |
| Ecosystem docs repo | [capysquash-docs](https://github.com/CAPYSQUASH/capysquash-docs) |

</div>

## Contributing

Contributions are welcome across the ecosystem.

<div align="center">

[![Contributors](https://img.shields.io/github/contributors/CAPYSQUASH/capysquash-cli.svg?logo=github)](https://github.com/CAPYSQUASH/capysquash-cli/graphs/contributors)
[![Issues](https://img.shields.io/github/issues/CAPYSQUASH/capysquash-platform.svg?logo=github)](https://github.com/CAPYSQUASH/capysquash-platform/issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/CAPYSQUASH/capysquash-platform.svg?logo=github)](https://github.com/CAPYSQUASH/capysquash-platform/pulls)

</div>

- Contribution guide: [`capysquash-cli/CONTRIBUTING.md`](https://github.com/CAPYSQUASH/capysquash-cli/blob/main/CONTRIBUTING.md)
- Security policy: [`capysquash-cli/SECURITY.md`](https://github.com/CAPYSQUASH/capysquash-cli/blob/main/SECURITY.md)

---

<div align="center">
  [![Website](https://img.shields.io/badge/Website-capysquash.dev-f97316?style=for-the-badge)](https://capysquash.dev)
  [![Docs](https://img.shields.io/badge/Docs-GitHub%20Docs-0EA5E9?style=for-the-badge)](https://github.com/CAPYSQUASH/capysquash-docs)

  <sub>Built by the CapySquash team 🟧</sub>
</div>
