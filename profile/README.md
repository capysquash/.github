<div align="center">
  <img src="https://raw.githubusercontent.com/CAPYSQUASH/capysquash-platform/main/public/icons/icon0.svg" alt="CapySquash" width="72" height="72" />

  # CAPYSQUASH

  **AI-native workflow acceleration for SQL + code changes**

  [![Platform](https://img.shields.io/badge/Platform-Next.js_16-000000?style=flat-square&logo=nextdotjs)](https://github.com/CAPYSQUASH/capysquash-platform)
  [![CLI](https://img.shields.io/badge/CLI-Go-00ADD8?style=flat-square&logo=go)](https://github.com/CAPYSQUASH/capysquash-cli)
  [![API](https://img.shields.io/badge/API-Go-00ADD8?style=flat-square&logo=go)](https://github.com/CAPYSQUASH/capysquash-api)
  [![Engine](https://img.shields.io/badge/Engine-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)](https://github.com/CAPYSQUASH/pgsquash-engine)
  [![Docs](https://img.shields.io/badge/Docs-Fumadocs-0EA5E9?style=flat-square)](https://github.com/CAPYSQUASH/capysquash-docs)
</div>

---

## Overview

CapySquash helps teams **ship database and app changes with confidence**.

We build an integrated ecosystem where CLI, API, engine, platform, and docs stay aligned—so you can move from planning to validation to rollout without context switching or fragile handoffs.

## What CapySquash gives you

<table>
<tr>
<td width="50%">

### Safer SQL delivery
- Environment-aware validation
- Migration risk checks before rollout
- Reviewable change workflows
- Operational guardrails and rollback thinking

</td>
<td width="50%">

### Faster developer flow
- One system across local + CI + production
- CLI, API, UI, and editor entrypoints
- Shared engine logic across products
- Documentation that maps to real workflows

</td>
</tr>
</table>

## Ecosystem map

### Core platform components

| Repository | Role |
|---|---|
| [`pgsquash-engine`](https://github.com/CAPYSQUASH/pgsquash-engine) | Core SQL/change intelligence engine used across products |
| [`capysquash-api`](https://github.com/CAPYSQUASH/capysquash-api) | Backend service exposing engine-backed operations |
| [`capysquash-cli`](https://github.com/CAPYSQUASH/capysquash-cli) | Local developer workflow entrypoint |
| [`capysquash-platform`](https://github.com/CAPYSQUASH/capysquash-platform) | Web app for orchestration, visibility, and team workflows |

### Developer surfaces

| Repository | Role |
|---|---|
| [`capysquash-studio`](https://github.com/CAPYSQUASH/capysquash-studio) | Web UI for management and operational workflows |
| [`capysquash-vscode`](https://github.com/CAPYSQUASH/capysquash-vscode) | VS Code extension for in-editor workflows |
| [`capysquash-docs`](https://github.com/CAPYSQUASH/capysquash-docs) | Product + technical documentation hub |
| [`homebrew-tap`](https://github.com/CAPYSQUASH/homebrew-tap) | Homebrew distribution for CLI installation |

### Adjacent initiatives

| Repository | Role |
|---|---|
| [`capydb`](https://github.com/CAPYSQUASH/capydb) | Framework-native Postgres initiative adjacent to the CapySquash ecosystem |

## How the system connects

```mermaid
flowchart LR
  CLI[capysquash-cli] --> API[capysquash-api]
  Platform[capysquash-platform] --> API
  Studio[capysquash-studio] --> API
  VSCode[capysquash-vscode] --> API
  API --> Engine[pgsquash-engine]
  Engine --> PG[(PostgreSQL)]
  Docs[capysquash-docs] -. guides .-> CLI
  Docs -. guides .-> Platform
```

## Start here

<table>
<tr>
<td align="center" width="33%">
<strong>Install & run locally</strong><br/>
Start with <a href="https://github.com/CAPYSQUASH/capysquash-cli/blob/main/GETTING_STARTED.md"><code>capysquash-cli/GETTING_STARTED.md</code></a>
</td>
<td align="center" width="33%">
<strong>Explore the web platform</strong><br/>
Read <a href="https://github.com/CAPYSQUASH/capysquash-platform/blob/main/README.md"><code>capysquash-platform/README.md</code></a>
</td>
<td align="center" width="33%">
<strong>Dive into docs</strong><br/>
Browse <a href="https://github.com/CAPYSQUASH/capysquash-docs"><code>capysquash-docs</code></a>
</td>
</tr>
</table>

## Contributing

We welcome issues and pull requests across the ecosystem.

- Contribution guide: [`capysquash-cli/CONTRIBUTING.md`](https://github.com/CAPYSQUASH/capysquash-cli/blob/main/CONTRIBUTING.md)
- Security policy: [`capysquash-cli/SECURITY.md`](https://github.com/CAPYSQUASH/capysquash-cli/blob/main/SECURITY.md)

---

<div align="center">
  <sub>Built by the CapySquash team 🟧</sub>
</div>