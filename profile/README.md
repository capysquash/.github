# CAPYSQUASH

<div align="center">

[![GitHub Stars](https://img.shields.io/github/stars/capysquash/pgsquash-engine?style=social)](https://github.com/capysquash/pgsquash-engine)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Go Version](https://img.shields.io/badge/go-%3E%3D1.21-brightgreen.svg)](https://go.dev/)
[![Discord](https://img.shields.io/discord/YOUR_DISCORD_ID?color=7289da&label=Discord&logo=discord&logoColor=white)](https://discord.gg/capysquash)

</div>

<div align="center">

<svg width="120" height="120" viewBox="0 0 120 120" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect x="10" y="30" width="100" height="70" rx="20" fill="#8B7355" stroke="#000000" stroke-width="6"/>
<circle cx="40" cy="50" r="8" fill="#000000"/>
<circle cx="80" cy="50" r="8" fill="#000000"/>
<path d="M35 70 Q60 80 85 70" stroke="#000000" stroke-width="4" fill="none" stroke-linecap="round"/>
<rect x="85" y="40" width="30" height="20" rx="4" fill="#FBBF24" stroke="#000000" stroke-width="3" transform="rotate(15 100 50)"/>
<text x="92" y="55" font-size="12" font-weight="bold" fill="#000000">SQL</text>
</svg>

**You ship fast, we clean the mess**

Automatic Postgres migration cleanup for developers who move fast.
Built for Supabase, Neon, and modern stacks.

</div>

Your migrations pile up. **We squash them automatically.**
Same schema. Cleaner history. Zero risk.

## Features

<table>
<tr>
<td align="center" width="50%">

<svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M13 3h-2v10h2V3zm4.83 2.17l-1.42 1.42C17.99 7.86 19 9.81 19 12c0 3.87-3.13 7-7 7s-7-3.13-7-7c0-2.19 1.01-4.14 2.58-5.42L6.17 5.17C4.23 6.82 3 9.26 3 12c0 4.97 4.03 9 9 9s9-4.03 9-9c0-2.74-1.23-5.18-3.17-6.83z" fill="#10B981"/>
</svg>

**⚡ Ship Faster**
Cut deploy times in half. 92 migrations → 12 migrations. Automatic consolidation.

</td>
<td align="center" width="50%">

<svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 1L3 5v6c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V5l-9-4zm-2 16l-4-4 1.41-1.41L10 14.17l6.59-6.59L18 9l-8 8z" fill="#6366F1"/>
</svg>

**🔒 Sleep Well**
Docker-validated safety. Parser-grade SQL analysis. 100% schema match guarantee.

</td>
</tr>
<tr>
<td align="center">

<svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zM9 17H7v-7h2v7zm4 0h-2V7h2v10zm4 0h-2v-4h2v4z" fill="#FBBF24"/>
</svg>

**🧹 Stay Clean**
Automatic consolidation. GitHub bot creates PRs. Review and merge when ready.

</td>
<td align="center">

<svg width="48" height="48" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z" fill="#67E8F9"/>
</svg>

**🤖 Just Merge**
One-click PRs. Automatic validation. No manual consolidation needed.

</td>
</tr>
</table>

## Quick Start

<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M4 12l1.41 1.41L11 7.83V20h2V7.83l5.58 5.59L20 12l-8-8-8 8z" fill="#059669"/>
</svg>

### Installation

```bash
# Install the CLI globally
npm install -g pgsquash

# Or use with Go
go install github.com/capysquash/pgsquash-engine/cmd/pgsquash@latest

# Or install the GitHub App
# → https://github.com/apps/capysquash
```

### Basic Usage

```bash
# Analyze your migration directory
pgsquash analyze

# Create squashed migrations
pgsquash squash --output ./squashed

# Interactive TUI mode
pgsquash interactive
```

That's it! Your migrations are cleaned up.

## How It Works

1. **Analyze**: Parses all SQL migrations using `pg_query_go` for accuracy
2. **Consolidate**: Groups related migrations intelligently (schema, data, indexes)
3. **Validate**: Spins up Docker containers to verify identical schema
4. **Create PR**: GitHub bot creates a reviewed, tested pull request

## The Problem vs The Solution

<table>
<tr>
<td width="50%">

### ❌ Before

```
migrations/
├── 0001_initial_schema.sql
├── 0002_add_users_table.sql
├── 0003_fix_typo_in_users.sql
├── 0004_add_email_column.sql
├── 0005_make_email_unique.sql
├── 0006_add_posts_table.sql
├── 0007_fix_posts_constraint.sql
├── ...
└── 0092_another_hotfix.sql

⏱️  8 minute deploys
😰 New dev setup: 2 hours
🐛 Flaky migrations
```

</td>
<td width="50%">

### ✅ After

```
migrations/
├── 0001_initial_schema.sql
├── 0002_users_and_auth.sql
├── 0003_posts_complete.sql
├── 0004_payments_system.sql
└── 0012_latest_features.sql



⚡ 3 minute deploys
😌 New dev setup: 5 minutes
✨ Rock solid
```

</td>
</tr>
</table>

## Supported Technologies

<div align="center">

<table>
<tr>
<td align="center">

<svg width="64" height="64" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2z" fill="#3ECF8E"/>
<path d="M12 8c-2.21 0-4 1.79-4 4s1.79 4 4 4 4-1.79 4-4-1.79-4-4-4z" fill="#FFFFFF"/>
</svg>

**Supabase**
Native migrations
Edge Functions
Real-time

</td>
<td align="center">

<svg width="64" height="64" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect x="4" y="4" width="16" height="16" rx="3" fill="#00E699"/>
<path d="M8 12h8M12 8v8" stroke="#000000" stroke-width="2"/>
</svg>

**Neon**
Branch-aware
Serverless
Autoscaling

</td>
<td align="center">

<svg width="64" height="64" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M21.8 10.5l-9.8-8.5-9.8 8.5h2.8v9.5h4v-6h6v6h4v-9.5h2.8z" fill="#2D3748"/>
</svg>

**Prisma**
Schema migrations
Type-safe
ORM integration

</td>
<td align="center">

<svg width="64" height="64" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<circle cx="12" cy="12" r="10" fill="#C5F74F"/>
<path d="M8 12l2 2 6-6" stroke="#000000" stroke-width="2" fill="none"/>
</svg>

**Drizzle**
SQL-like syntax
TypeScript-first
Zero dependencies

</td>
</tr>
</table>

Also supports: **TypeORM** • **Knex.js** • **Sequelize** • **Native SQL** • **Any Postgres migration tool**

</div>

## Core Commands

<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2z" fill="#374151"/>
<path d="M4 8h16M4 12h8M4 16h12" stroke="#FFFFFF" stroke-width="1.5"/>
</svg>

```bash
# Analysis & Planning
pgsquash analyze                     # Analyze migration history
pgsquash analyze --verbose           # Show detailed analysis
pgsquash stats                       # Show migration statistics

# Squashing Operations
pgsquash squash                      # Create squashed migrations
pgsquash squash --aggressive         # More aggressive consolidation
pgsquash squash --dry-run            # Preview without changes

# Validation
pgsquash validate                    # Validate squashed migrations
pgsquash validate --postgres 15      # Test specific Postgres version
pgsquash docker-test                 # Full Docker validation

# Interactive
pgsquash interactive                 # TUI mode for visual management
pgsquash tui                         # Alias for interactive

# Utilities
pgsquash init                        # Initialize config file
pgsquash config                      # Show current configuration
pgsquash version                     # Show version info
```

## Configuration

```json
{
  "migrations": {
    "directory": "./migrations",
    "pattern": "*.sql",
    "naming": "timestamp"
  },
  "squash": {
    "safetyLevel": "conservative",
    "groupStrategy": "semantic",
    "maxFilesPerGroup": 50
  },
  "validation": {
    "dockerImage": "postgres:15-alpine",
    "runTests": true,
    "compareSchemas": true
  }
}
```

## Examples

### Basic Project Cleanup

```bash
# Initialize in your project
cd my-project
pgsquash init

# Analyze your migrations
pgsquash analyze

# Create squashed version
pgsquash squash --output ./squashed

# Validate the results
pgsquash validate
```

### GitHub App Workflow

```bash
# 1. Install GitHub App
# → https://github.com/apps/capysquash

# 2. CAPYSQUASH analyzes your repo automatically

# 3. Receive PR when cleanup is recommended
# → Review changes in PR
# → Validate in CI
# → Merge when ready

# 4. Your migrations are now clean!
```

### CI/CD Integration

```yaml
# .github/workflows/migrations.yml
name: Migration Cleanup

on:
  schedule:
    - cron: '0 0 * * 0' # Weekly

jobs:
  squash:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Install pgsquash
        run: npm install -g pgsquash
      - name: Analyze migrations
        run: pgsquash analyze --json > analysis.json
      - name: Create PR if needed
        run: pgsquash squash --create-pr
```

## 📊 By The Numbers

<div align="center">

```
╔════════════════════════════════════════╗
║  🗂  92 → 12 files     ✨ 87% cleaner  ║
║  ⏱  8m → 3m deploys    🚀 62% faster   ║
║  ✅  100% schema match  🔒 Zero risk    ║
║  🐳  Docker validated   😌 Sleep well   ║
╚════════════════════════════════════════╝
```

</div>

## Our Projects

<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2L2 7v10c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V7l-10-5z" fill="#8B5CF6"/>
</svg>

### [`pgsquash-engine`](https://github.com/capysquash/pgsquash-engine)
**The open-source CLI.** Powerful, local-first, built for developers.

- ⚡ Parser-grade SQL analysis with `pg_query_go`
- 🐳 Docker-based validation (tests your actual Postgres version)
- 🎨 Beautiful TUI for interactive cleanup
- 🎯 Safety levels: conservative to aggressive
- 🆓 100% free, 100% open source
- 🏗️ Written in Go for speed and reliability

### [`capysquash-platform`](https://github.com/capysquash/capysquash-platform)
**The collaboration SaaS.** For teams and agencies who need more.

- 🤖 GitHub App with automated PRs
- 📊 Multi-project dashboard
- 👥 Team roles & permissions
- 📝 White-label client reports
- 🔗 Deployment integrations (Vercel, Railway, Render)
- 📈 Migration health analytics across all projects

## Roadmap

<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20 6h-2.18c.11-.31.18-.65.18-1a2.996 2.996 0 0 0-5.5-1.65l-.5.67-.5-.68C10.96 2.54 10.05 2 9 2 7.34 2 6 3.34 6 5c0 .35.07.69.18 1H4c-1.11 0-1.99.89-1.99 2L2 19c0 1.11.89 2 2 2h16c1.11 0 2-.89 2-2V8c0-1.11-.89-2-2-2z" fill="#0891B2"/>
</svg>

- [x] **Core Engine** - Parser + Docker validation ✅
- [x] **GitHub App** - Automated PR workflow ✅
- [x] **Supabase Support** - Native integration ready ✅
- [x] **Neon Support** - Branch-aware analysis ✅
- [ ] **VS Code Extension** - Real-time migration linting (Q1 2026)
- [ ] **Vercel Integration** - Build time insights (Q1 2026)
- [ ] **Supabase CLI Plugin** - `supabase pgsquash` command (Q2 2026)
- [ ] **Team Analytics** - Migration health dashboards (Q2 2026)
- [ ] **AI-Powered Suggestions** - Smart grouping recommendations (Q3 2026)

**[→ Full Roadmap & Discussion](https://github.com/capysquash/pgsquash-engine/discussions)**

## Documentation

<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8l-6-6z" fill="#6366F1"/>
<path d="M14 2v6h6" fill="none" stroke="#FFFFFF" stroke-width="2"/>
</svg>

- **[Getting Started](https://capysquash.dev/docs/getting-started)** - Complete setup guide
- **[CLI Reference](https://capysquash.dev/docs/cli)** - All commands and options
- **[Configuration](https://capysquash.dev/docs/configuration)** - Advanced settings
- **[GitHub App Guide](https://capysquash.dev/docs/github-app)** - Automated workflow
- **[Best Practices](https://capysquash.dev/docs/best-practices)** - Migration strategies
- **[Troubleshooting](https://capysquash.dev/docs/troubleshooting)** - Common issues

## Philosophy

We believe:

- **🚀 Ship fast > ship perfect** – Iteration beats perfection
- **🤖 Automation > manual work** – Your time is valuable
- **🔒 Safety > speed** – But you can have both
- **💚 Open source > closed** – Great tools should be free
- **😎 Vibes > corporate speak** – We're developers, not sales
- **🦫 Chill > chaos** – Migration cleanup should be calm

## Contributing

<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16 1H4c-1.1 0-2 .9-2 2v14h2V3h12V1zm3 4H8c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h11c1.1 0 2-.9 2-2V7c0-1.1-.9-2-2-2zm0 16H8V7h11v14z" fill="#7C3AED"/>
</svg>

We welcome contributions! CAPYSQUASH is built by developers, for developers.

- 🐛 [Report bugs](https://github.com/capysquash/pgsquash-engine/issues/new?template=bug_report.md)
- 💡 [Request features](https://github.com/capysquash/pgsquash-engine/issues/new?template=feature_request.md)
- 📖 [Improve documentation](https://github.com/capysquash/capysquash-docs)
- 🔧 [Submit pull requests](https://github.com/capysquash/pgsquash-engine/pulls)
- 💬 [Join discussions](https://github.com/capysquash/pgsquash-engine/discussions)

**[→ Contributing Guide](https://github.com/capysquash/pgsquash-engine/blob/main/CONTRIBUTING.md)**

## Requirements

<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M20 18c1.1 0 1.99-.9 1.99-2L22 5c0-1.1-.9-2-2-2H4c-1.1 0-2 .9-2 2v11c0 1.1.9 2 2 2H0c0 1.1.9 2 2 2h20c1.1 0 2-.9 2-2h-4z" fill="#6B7280"/>
</svg>

**For CLI:**
- **Go**: >= 1.21 (if building from source)
- **Node.js**: >= 18.0.0 (if using npm package)
- **Docker**: >= 20.10 (for validation)
- **Postgres**: Any version (we test against 12-16)

**For GitHub App:**
- Just install it. No requirements.

## 🦫 Why a Capybara?

Because capybaras are:
- **😌 Chill** – Famously calm, like automation should be
- **🧹 Helpful** – They clean up (literally, in nature)
- **🤝 Team players** – Get along with everyone (just like our integrations)
- **🌟 Internet gold** – Beloved by developers everywhere

Plus, we needed a mascot. Docker has a whale. We have a capybara. **Deal with it.** 😎

## License

<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8l-6-6z" fill="#9CA3AF"/>
<path d="M14 2v6h6" fill="none" stroke="white" stroke-width="2"/>
<text x="7" y="16" font-size="8" fill="#FFFFFF">MIT</text>
</svg>

**MIT License** - see the [LICENSE](https://github.com/capysquash/pgsquash-engine/blob/main/LICENSE) file for details.

The [`pgsquash-engine`](https://github.com/capysquash/pgsquash-engine) is 100% open source.
The [`capysquash-platform`](https://github.com/capysquash/capysquash-platform) SaaS is source-available for transparency.

**Free forever. Use anywhere. Build anything.**

## Support & Community

<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z" fill="#059669"/>
</svg>

- 💬 **Discord**: [Join our community](https://discord.gg/capysquash) - Get help, share wins
- 🐦 **Twitter**: [@capysquash](https://twitter.com/capysquash) - Updates & memes
- 📧 **Email**: hello@capysquash.dev - Business inquiries
- 📚 **Docs**: [capysquash.dev](https://capysquash.dev) - Complete documentation
- 🐛 **Issues**: [GitHub Issues](https://github.com/capysquash/pgsquash-engine/issues) - Bug reports & features

## Built For

<table>
<tr>
<td width="25%" align="center">

**🎨 Vibe Coders**
Keep your momentum
We handle the mess

</td>
<td width="25%" align="center">

**🚀 Startups**
Onboard in minutes
Not hours

</td>
<td width="25%" align="center">

**🏢 Agencies**
Multi-project
White-label reports

</td>
<td width="25%" align="center">

**🔧 Engineers**
Parser-grade accuracy
Docker validation

</td>
</tr>
</table>

---

<div align="center">

## Ship fast. Stay clean. 🦫

**[Get Started](https://capysquash.dev)** · **[Install GitHub App](https://github.com/apps/capysquash)** · **[Read Docs](https://capysquash.dev/docs)** · **[Join Discord](https://discord.gg/capysquash)**

<sub>Built with ❤️ by developers who got tired of migration hell</sub>

</div>
