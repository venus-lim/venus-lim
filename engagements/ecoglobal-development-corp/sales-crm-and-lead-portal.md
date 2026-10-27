# EcoGlobal Sales & Marketing CRM Portal (`ecoglobal-sales-portal`)

**Company:** EcoGlobal Development Corp.  
**Repository Visibility:** Private (`423` files · `61` commits · 12-folder `docs/` tree)

---

### 1. System Purpose
A standalone internal property sales and marketing CRM built to track real-estate inquiries, sales pipelines, and follow-up workflows for EcoGlobal Development Corp.

---

### 2. Monorepo Structure & Connected Platforms
```text
ecoglobal-sales-portal/
├── CLAUDE.md & ENV.md   Project rules & Doppler environment variable safety directive
├── client/              React + Vite frontend deployed via Render Static Sites
├── server/              Express.js API backend deployed on Render
├── design-system/       Isolated visual UI sandbox (no live API connections)
├── database/prisma/     Prisma schema & local test database migrations
├── toolbelt/            Internal utility scripts
└── docs/                12-folder business logic, UI specs & workflow documentation
```

* **Supabase (`PostgreSQL`):** Cloud database managed through Prisma schema definitions, paired with a local Postgres test replica so tests never run against live data.
* **Render & Render Static Sites:** Separate hosting targets for the `server/` API backend and `client/` React frontend.
* **Doppler:** Centralized secret management (`ENV.md` rules block `.env` credential files from ever being stored in the repository).
* **Brevo:** Automated transactional email integration.
