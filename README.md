# Venus Lim

Operations, AI workflow systems, and creative production.  
Quezon City, PH · [limvenus167@gmail.com](mailto:limvenus167@gmail.com)

I build internal operations tools, conversion storefronts, and short-form video pipelines. Instead of one-shot prompting, I structure repositories around linked Markdown context graphs (`CLAUDE.md` + `docs/`) and modular task breakdowns so AI agents (`Claude Code`, `Antigravity`) execute against defined business rules before human QA and post-production engineering sign-off.

---

### Languages, Platforms & Integrations

* **Languages & Formats:** JavaScript (`Node.js`, ES Modules), Google Apps Script (`.gs`), SQL (`PostgreSQL`), HTML5, CSS3 (`Tailwind CSS`), React (`JSX`), Prisma Schema, Markdown (`.md`)
* **Cloud, Hosting & Databases:** Supabase (`PostgreSQL`, `Auth`, `Storage`), Cloudflare Pages (`Wrangler`), Render (`Web Services` & `Render Static Sites`), Doppler (environment secrets), GoDaddy (custom domains & DNS)
* **Workspace & Messaging Integrations:** Google Workspace (`Sheets`, `Drive`, `Docs` synced via `clasp` CLI), Brevo (automated transactional email & HTML templates), Meta Lead Webhooks
* **AI & Context Tooling:** Claude (`Native Desktop App`, `VS Code`, `Supervised Terminal CLI`), Google Antigravity, Obsidian (`graphify` linked context graphs), task-based model routing (`Haiku` · `Sonnet` · `Opus`)
* **Video & Creative Pipeline:** Adobe Premiere Pro (`.prproj`, `.mogrt`), CapCut, Adobe Media Encoder (`9:16` vertical & `16:9` batch exports), Canva Pro, Meta Business Suite

---

### Repositories by Company

Production repositories are kept private to protect client records and internal business logic. Sanitized architectural briefs and live deployments are linked below:

**EcoGlobal Development Corp.** *(1-year contractual span — [multi-system overview](./engagements/ecoglobal-development-corp/README.md))*
* `ecoglobal-leasing-operations` — **Leasing Operations Platform** · 11-hub property, billing, and tenancy system (`1,241` files, `289` context docs) · [architecture spec](./engagements/ecoglobal-development-corp/leasing-operations-platform.md) · [condormitel.homes](https://condormitel.homes)
* `ecoglobal-workspace-automations` — **Workspace & Apps Script Console (`v318 STAFF LIVE`)** · Daily staff operations console, monthly ledger automation, and local `clasp` verification mirror (`1,699` files, `138` deployed script files) · [architecture spec](./engagements/ecoglobal-development-corp/workspace-apps-script-console.md)
* `ecoglobal-sales-portal` — **Sales & Lead CRM Portal** · Property inquiry pipeline connected to `condormitel.homes`, Meta lead webhooks, Supabase, Render, and Brevo (`423` files) · [architecture spec](./engagements/ecoglobal-development-corp/sales-crm-and-lead-portal.md)

**Planet of the Capes**
* `planet-of-the-capes-storefront` — **Collector Storefront & Catalog Showcase** · Modular web storefront (`sections/00–08` compiled via Node `build.js`), embedded video reels, category filter tabs, and interactive "Dibs" claim preview (`422` files) · [architecture spec](./engagements/planet-of-the-capes/storefront-and-catalog.md) · [planetofthecapes.shop](https://planetofthecapes.shop) *(live preview)*

**TrueGrit**
* `truegrit-landing-page` — **Conversion Landing Page** · Responsive digital storefront and lead-capture layout · [architecture spec](./engagements/truegrit/conversion-landing-page.md)

---

### Standard Repository Architecture

Every full-stack repository separates business rules and audit logs (`docs/`) from live application code:

```text
project-repository/
├── CLAUDE.md                  Root project manual: rules, workflows & folder index
├── docs/ (what · how · when)  Business logic, architecture, logs, audits & plans (.md)
├── Frontend/ & design-system/ Live web UI + isolated visual preview sandbox
├── Backend/ (or server/)      API routes, webhook listeners & business services
├── Database/ (prisma/)        PostgreSQL schema & chronological SQL migrations
└── .claude/ & .agents/skills/ Reusable AI agent workflows, rules & check scripts
```

Full workflow overview: [Context Architecture & Sub-Charger Workflow](./context-architecture/repository-blueprint.md)

---

*Scope & Engineering Sign-Off: I do not claim formal Computer Science credentials. I map the business workflows, curate the repository context, and assemble the working modules using AI tooling—after which production codebases undergo review and final sign-off by a Senior Licensed Computer Engineer post-production.*
