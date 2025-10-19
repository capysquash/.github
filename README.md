# 🦫 CAPYSQUASH

> **You ship fast, we clean the mess**

Automatic Postgres migration cleanup for developers who move fast.  
Built for Supabase, Neon, and modern stacks.

---

## What We Do

Your migrations pile up. **We squash them automatically.**

- ⚡ **Ship faster** – Cut deploy times in half
- 🧹 **Stay clean** – 92 files → 12 files, automatically
- 🔒 **Sleep well** – Docker-validated safety, zero risk
- 🤖 **Just merge** – GitHub bot creates one-click PRs

<br>

## The Problem

```diff
- migrations/
-   0001_initial_schema.sql
-   0002_add_users_table.sql
-   0003_fix_typo_in_users.sql
-   0004_add_email_to_users.sql
-   0005_make_email_unique.sql
-   ...
-   0092_another_quick_fix.sql
```

Every migration adds deployment overhead. Your CI gets slower. Your database setup gets flakier. Your new devs spend hours debugging local environments.

**This is normal.** You're shipping fast. That's good.

<br>

## The Solution

```diff
+ migrations/
+   0001_initial_schema.sql
+   0002_users_and_auth.sql
+   0003_payments_complete.sql
+   ...
+   0012_latest_features.sql
```

CAPYSQUASH consolidates your migration history automatically. Same final schema. Cleaner history. Faster deploys.

**The best part?** It happens in a GitHub PR. Review. Merge. Done.

<br>

---

<br>

## 🚀 Quick Start

### Install GitHub App (Recommended)

The easiest way. CAPYSQUASH analyzes your repo, creates PRs automatically.

**[→ Install GitHub App](https://github.com/apps/capysquash)**

### Use the CLI

For local control or CI/CD integration.

```bash
# Install
npm install -g pgsquash

# Analyze your migrations
pgsquash analyze

# Create a squashed version
pgsquash squash --output ./squashed
```

**[→ Read the docs](https://capysquash.dev/docs)**

<br>

---

<br>

## 💡 Built For

### 🎨 Vibe Coders & Indie Hackers
Keep your momentum. We handle the database mess.

### 🚀 Startups & Growing Teams  
Onboard new engineers in minutes, not hours. No more migration hell.

### 🏢 Agencies
Deliver clean, professional databases to every client. Multi-project management built in.

### 🔧 Backend Specialists
Parser-grade accuracy with `pg_query_go`. Docker validation on every squash.

<br>

---

<br>

## 🛠 Works With Everything

<table>
<tr>
<td align="center" width="25%">
<img src="https://avatars.githubusercontent.com/u/54469796?s=200&v=4" width="80" height="80" alt="Supabase"/>
<br><strong>Supabase</strong>
</td>
<td align="center" width="25%">
<img src="https://avatars.githubusercontent.com/u/77770362?s=200&v=4" width="80" height="80" alt="Neon"/>
<br><strong>Neon</strong>
</td>
<td align="center" width="25%">
<img src="https://avatars.githubusercontent.com/u/17219288?s=200&v=4" width="80" height="80" alt="Prisma"/>
<br><strong>Prisma</strong>
</td>
<td align="center" width="25%">
<img src="https://avatars.githubusercontent.com/u/22247014?s=200&v=4" width="80" height="80" alt="Drizzle"/>
<br><strong>Drizzle</strong>
</td>
</tr>
</table>

Native migrations, TypeORM, Knex, Sequelize – **if it's Postgres SQL files, we handle it.**

<br>

---

<br>

## 📊 By The Numbers

```
🗂  92 → 12 files        ✨ 87% cleaner
⏱  8m → 3m deploys       🚀 62% faster  
✅  100% schema match     🔒 Zero risk
🐳  Docker validated      😌 Sleep well
```

<br>

---

<br>

## 🏗 Our Stack

### [`pgsquash-engine`](https://github.com/capysquash/pgsquash-engine)
**The open-source CLI.** Powerful, local-first, built for developers.

- Parser-grade SQL analysis with `pg_query_go`
- Docker-based validation (your actual Postgres version)
- TUI for interactive cleanup
- Safety levels: conservative to aggressive
- 100% free, 100% open source

### [`capysquash-platform`](https://github.com/capysquash/capysquash-platform)
**The collaboration SaaS.** For teams and agencies.

- GitHub App with automated PRs
- Multi-project dashboard
- Team roles & permissions
- White-label client reports
- Deployment integrations (Vercel, Railway, Render)

<br>

---

<br>

## 🎯 Roadmap

- [x] **Core Engine** – Parser + Docker validation
- [x] **GitHub App** – Automated PR workflow
- [x] **Supabase Support** – Native integration ready
- [x] **Neon Support** – Branch-aware analysis
- [ ] **VS Code Extension** – Real-time migration linting
- [ ] **Vercel Integration** – Build time insights
- [ ] **Supabase CLI Plugin** – `supabase pgsquash` command
- [ ] **Team Analytics** – Migration health across projects

**[→ Full Roadmap](https://github.com/capysquash/pgsquash-engine/blob/main/ROADMAP.md)**

<br>

---

<br>

## 🌟 Philosophy

We believe:

- **Ship fast > ship perfect** – Iteration beats perfection
- **Automation > manual work** – Your time is valuable  
- **Safety > speed** – But you can have both
- **Open source > closed** – Great tools should be free
- **Vibes > corporate speak** – We're developers, not sales

<br>

---

<br>

## 🤝 Community

- **Discord**: [Join the server](https://discord.gg/capysquash) – Get help, share wins
- **Twitter**: [@capysquash](https://twitter.com/capysquash) – Updates & memes
- **Docs**: [capysquash.dev](https://capysquash.dev) – Guides & API reference

<br>

---

<br>

## 🦫 Why a Capybara?

Because capybaras are:
- **Chill** – Famously calm, like automation should be
- **Helpful** – They clean up (literally, in nature)
- **Team players** – Get along with everyone
- **Internet gold** – You know you love them

Plus, we needed a mascot. Docker has a whale. We have a capybara. **Deal with it.** 😎

<br>

---

<br>

## 📄 License

**MIT License** – Free forever, use anywhere, build anything.

The [`pgsquash-engine`](https://github.com/capysquash/pgsquash-engine) is 100% open source.  
The [`capysquash-platform`](https://github.com/capysquash/capysquash-platform) SaaS is source-available for transparency.

<br>

---

<br>

<div align="center">

## Ship fast. Stay clean. 🦫

**[Get Started](https://capysquash.dev)** · **[Install GitHub App](https://github.com/apps/capysquash)** · **[Read Docs](https://capysquash.dev/docs)**

<sub>Built with ❤️ by developers who got tired of migration hell</sub>

</div>
