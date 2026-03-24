<div align="center">
  <img src="https://raw.githubusercontent.com/CAPYSQUASH/capysquash-platform/main/public/icons/icon0.svg" alt="CapySquash" width="80" height="80" />

  # CAPYSQUASH

  **From migration clutter to clean, shippable history.**

  [![Platform](https://img.shields.io/badge/Platform-Next.js-000000?style=flat-square&logo=nextdotjs)](https://github.com/CAPYSQUASH/capysquash-platform)
  [![CLI](https://img.shields.io/badge/CLI-Go-00ADD8?style=flat-square&logo=go)](https://github.com/CAPYSQUASH/capysquash-cli)
  [![API](https://img.shields.io/badge/API-Go-00ADD8?style=flat-square&logo=go)](https://github.com/CAPYSQUASH/capysquash-api)
  [![Engine](https://img.shields.io/badge/Engine-pgsquash--engine-4169E1?style=flat-square&logo=postgresql&logoColor=white)](https://github.com/CAPYSQUASH/pgsquash-engine)
  [![Docs](https://img.shields.io/badge/Docs-Fumadocs-0EA5E9?style=flat-square)](https://github.com/CAPYSQUASH/capysquash-docs)
</div>

---

## Why CapySquash exists

Databases don’t usually break in one dramatic moment.
They drift.

One migration here, one hotfix there, one “we’ll clean it later” at 2 a.m.—and suddenly shipping schema changes feels like defusing a bomb with a sticky note.

**CapySquash is built to fix that feeling.**

We help developers consolidate migration debt, reduce risk, and ship faster with clearer SQL history and safer workflows.

## The product model (intentionally simple)

CapySquash is the primary product and brand.

- **`capysquash-platform`** is the main experience (dashboard + automation).
- **`capysquash-cli`** and **`capysquash-api`** are supporting surfaces.
- **`pgsquash-engine`** is the core technology under the hood.

Different entrypoints. One system.

## What you get

<table>
<tr>
<td width="50%">

### ✅ Safer database changes
- Analyze before you apply
- Catch risky migration patterns early
- Keep schema evolution reviewable
- Build confidence from local to production

</td>
<td width="50%">

### ⚡ Faster shipping loops
- Platform + CLI + API stay aligned
- Automation-ready workflows for teams and solo devs
- Shared engine behavior across every surface
- Docs that map to how people actually build

</td>
</tr>
</table>

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

## How work flows through CapySquash

1. **Prepare** changes in your local workflow (CLI/editor/platform).
2. **Analyze** and validate through API + engine capabilities.
3. **Ship** with clearer history, better guardrails, and fewer surprises.

## Where to start

| If you want to... | Start here |
|---|---|
| Use the main product experience | [`capysquash-platform`](https://github.com/CAPYSQUASH/capysquash-platform) |
| Work from terminal/CI | [`capysquash-cli/GETTING_STARTED.md`](https://github.com/CAPYSQUASH/capysquash-cli/blob/main/GETTING_STARTED.md) |
| Integrate over HTTP | [`capysquash-api/README.md`](https://github.com/CAPYSQUASH/capysquash-api/blob/main/README.md) |
| Explore full documentation | [`capysquash-docs`](https://github.com/CAPYSQUASH/capysquash-docs) |

## Contributing

Contributions are welcome across the ecosystem.

- Contribution guide: [`capysquash-cli/CONTRIBUTING.md`](https://github.com/CAPYSQUASH/capysquash-cli/blob/main/CONTRIBUTING.md)
- Security policy: [`capysquash-cli/SECURITY.md`](https://github.com/CAPYSQUASH/capysquash-cli/blob/main/SECURITY.md)

---

<div align="center">
  <sub>Built by the CapySquash team 🟧</sub>
</div>