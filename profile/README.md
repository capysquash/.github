<div align="center">

<svg width="1040" height="280" viewBox="0 0 1040 280" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="CapySquash banner">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1040" y2="280" gradientUnits="userSpaceOnUse">
      <stop stop-color="#111827"/>
      <stop offset="1" stop-color="#1F2937"/>
    </linearGradient>
    <linearGradient id="accent" x1="80" y1="30" x2="960" y2="250" gradientUnits="userSpaceOnUse">
      <stop stop-color="#F59E0B"/>
      <stop offset="1" stop-color="#22C55E"/>
    </linearGradient>
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="8" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <rect width="1040" height="280" rx="20" fill="url(#bg)"/>
  <path d="M0 210C180 170 320 248 520 210C720 172 860 252 1040 208V280H0V210Z" fill="url(#accent)" fill-opacity="0.25"/>
  <path d="M0 230C180 190 320 266 520 228C720 190 860 266 1040 224V280H0V230Z" fill="url(#accent)" fill-opacity="0.15"/>

  <g transform="translate(90,70)" filter="url(#glow)">
    <ellipse cx="90" cy="95" rx="88" ry="52" fill="#F59E0B"/>
    <ellipse cx="66" cy="78" rx="30" ry="22" fill="#FBBF24"/>
    <ellipse cx="144" cy="95" rx="18" ry="12" fill="#111827" opacity="0.22"/>
    <circle cx="70" cy="78" r="3.5" fill="#111827"/>
    <circle cx="88" cy="78" r="3.5" fill="#111827"/>
    <ellipse cx="79" cy="88" rx="6" ry="4" fill="#111827"/>
    <path d="M53 112Q90 128 128 112" stroke="#111827" stroke-width="4" stroke-linecap="round"/>
  </g>

  <text x="280" y="116" fill="white" font-family="ui-sans-serif, -apple-system, Segoe UI, Inter, Arial" font-size="56" font-weight="800" letter-spacing="0.2">CapySquash</text>
  <text x="282" y="160" fill="#D1D5DB" font-family="ui-sans-serif, -apple-system, Segoe UI, Inter, Arial" font-size="24" font-weight="500">AI-native workflow acceleration for SQL + code changes</text>
</svg>

</div>

<div align="center">

[![Docs](https://img.shields.io/badge/docs-fumadocs-0EA5E9?style=flat-square)](https://github.com/capysquash/capysquash-docs)
[![Platform](https://img.shields.io/badge/platform-next.js_16-000000?style=flat-square&logo=nextdotjs)](https://github.com/capysquash/capysquash-platform)
[![CLI](https://img.shields.io/badge/cli-go-00ADD8?style=flat-square&logo=go)](https://github.com/capysquash/capysquash-cli)
[![API](https://img.shields.io/badge/api-go-00ADD8?style=flat-square&logo=go)](https://github.com/capysquash/capysquash-api)
[![Engine](https://img.shields.io/badge/engine-postgres-orange?style=flat-square&logo=postgresql)](https://github.com/capysquash/pgsquash-engine)

</div>

---

CapySquash helps teams ship safer database and application changes with AI-assisted planning, validation, and rollout.

We focus on reducing migration risk, shortening review cycles, and keeping tooling aligned across local workflows, CI, and production.

## What we build

- **Safer SQL changes** with environment-aware checks and validation.
- **Faster delivery** through CLI/API/UI workflows designed to work together.
- **Production confidence** with guardrails, reviewability, and operational visibility.

## Ecosystem map

| Repository | Role |
|------------|------|
| [`capysquash-platform`](https://github.com/capysquash/capysquash-platform) | Web platform (dashboard, workflows, orchestration) |
| [`capysquash-cli`](https://github.com/capysquash/capysquash-cli) | Local developer CLI and automation entrypoint |
| [`capysquash-api`](https://github.com/capysquash/capysquash-api) | Backend services and API surface |
| [`pgsquash-engine`](https://github.com/capysquash/pgsquash-engine) | Core engine for SQL transformation/validation |
| [`capysquash-docs`](https://github.com/capysquash/capysquash-docs) | Product and technical documentation |
| [`capydb`](https://github.com/capysquash/capydb) | Data layer and storage-oriented components |
| [`capysquash-vscode`](https://github.com/capysquash/capysquash-vscode) | VS Code integration and editor workflows |
| [`homebrew-tap`](https://github.com/capysquash/homebrew-tap) | Homebrew distribution for CLI installation |

## How the pieces fit

1. Author or inspect change plans in **CLI** / **Platform**.
2. Validate and execute via **API** + **Engine**.
3. Keep teams aligned through **Docs** and editor integrations.

Same system, different entrypoints — no “shipcopter” layers required.

## Start here

- New to the ecosystem? Begin with [`capysquash-cli/GETTING_STARTED.md`](https://github.com/capysquash/capysquash-cli/blob/main/GETTING_STARTED.md)
- Want the platform view? See [`capysquash-platform/README.md`](https://github.com/capysquash/capysquash-platform/blob/main/README.md)
- Looking for implementation docs? Browse [`capysquash-docs`](https://github.com/capysquash/capysquash-docs)

## Contributing

We welcome issues, ideas, and pull requests across the ecosystem.

- Contribution guide: [`capysquash-cli/CONTRIBUTING.md`](https://github.com/capysquash/capysquash-cli/blob/main/CONTRIBUTING.md)
- Security reporting: [`capysquash-cli/SECURITY.md`](https://github.com/capysquash/capysquash-cli/blob/main/SECURITY.md)

---

<div align="center">
  <sub>Built by the CapySquash team 🟧</sub>
</div>