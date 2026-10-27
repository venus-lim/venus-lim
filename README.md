# Venus Lim

Operations, AI workflows, and creative production.  
Quezon City, PH · [limvenus167@gmail.com](mailto:limvenus167@gmail.com)

I build internal operations dashboards, web storefronts, and Google Workspace automations, alongside short-form video and creative production. Instead of one-shot prompting, I organize repositories around linked Markdown context files (`CLAUDE.md` + `docs/`) and modular task breakdowns so AI tools (`Claude Code`, `Antigravity`) work against defined business rules before human QA and post-production engineering review.

---

### Languages, Platforms & Tools

* **Languages & Formats:** JavaScript (`Node.js`), Google Apps Script (`.gs`), HTML/CSS (`Tailwind CSS`), React (`Vite`), SQL (`PostgreSQL` / `Prisma`), Markdown (`.md`)
* **Cloud & Hosting Platforms:** Supabase (`PostgreSQL` database & file storage), Render (`Web Services` & `Render Static Sites`), Cloudflare Pages, Doppler (environment variable management), GoDaddy (custom domains & DNS)
* **Workspace & Email Automations:** Google Workspace (`Sheets`, `Drive`, `Docs` synced via `clasp` CLI), Brevo (automated transactional email), Meta Lead Webhooks
* **AI & Context Workflow:** Claude (`Native Desktop App`, `VS Code`, `Supervised Terminal CLI`), Google Antigravity, Obsidian (`graphify` linked context docs), task-based model selection (`Haiku` · `Sonnet` · `Opus`)
* **Video Editing & Creative Tools:** Adobe Premiere Pro (`.prproj`, `.mogrt`), CapCut, Adobe Media Encoder (`9:16` & `16:9` exports), Canva Pro, Meta Business Suite

---

### Repositories by Company

Production repositories are kept private to protect client records and internal business logic. Sanitized overviews and live links are indexed below:

**EcoGlobal Development Corp.** *(1-year contractual span — [project overview](./engagements/ecoglobal-development-corp/README.md))*
* `ecoglobal-leasing-operations` — **Leasing Operations Dashboard** · 11-section property, utility billing, and tenancy management platform (`React`, `Vite`, `Express`, `Prisma`, `Supabase`) — `1,241` files, `289` context docs · [project spec](./engagements/ecoglobal-development-corp/leasing-operations-platform.md)
* `ecoglobal-workspace-automations` — **Workspace & Apps Script Console (`v318 STAFF LIVE`)** · Daily Google Sheets/Apps Script operations console (`138` deployed files), plus pulled workspace scripts including the **[condormitel.homes](https://condormitel.homes)** public inquiry page (`test-condormitel-homes-LIVE`) and `meta-leads-webhook` (`1,699` total files) · [project spec](./engagements/ecoglobal-development-corp/workspace-apps-script-console.md)
* `ecoglobal-sales-portal` — **Sales & Marketing CRM Portal** · Standalone property sales and lead tracking web application (`client/` on Render Static Sites, `server/` on Render, `database/prisma/` on Supabase, secrets in Doppler) — `423` files, 12-folder `docs/` tree · [project spec](./engagements/ecoglobal-development-corp/sales-crm-and-lead-portal.md)

**Planet of the Capes**
* `planet-of-the-capes-storefront` — **Collector Storefront & Catalog Showcase** · Modular web storefront (`sections/00–08` compiled via Node `build.js`), embedded video reels, category filter tabs, and interactive "Dibs" claim preview (`422` files) · [project spec](./engagements/planet-of-the-capes/storefront-and-catalog.md) · [planetofthecapes.shop](https://planetofthecapes.shop) *(live preview — under active development)*

**True Grit Studio**
* `truegrit-landing-page` — **Multi-View Landing Page** · Responsive web presentation (`discover`, `explore`, and `learn-more` views) built with modular HTML, CSS, and JavaScript · [project spec](./engagements/truegrit/conversion-landing-page.md)

---

### Standard Repository Structure

Full-stack repositories separate business rules and reference logs (`docs/`) from live application code:

```text
project-repository/
├── CLAUDE.md              Root project manual: operational rules, workflows & folder index
├── docs/                  Business logic, system architecture, audit logs & task plans (.md)
├── client/                Live web application (React, Vite, Tailwind CSS; or Frontend/)
├── server/                API services, webhook listeners & business logic (or Backend/)
├── database/              PostgreSQL schema, Prisma models & migrations (or Database/)
├── design-system/         Isolated visual sandbox for UI component staging & review
├── tests/                 Automated endpoint, schema, and integration verification suites
└── .claude/               AI agent workspace instructions, slash commands & check scripts
```

Workflow details: [Context Architecture & Modular Task Breakdown](./context-architecture/repository-blueprint.md)

---

*Scope & Engineering Sign-Off: I do not claim formal Computer Science credentials. I map the business workflows, organize the context files, and assemble the working modules using AI tooling—after which every production codebase undergoes review and final sign-off by a Senior Licensed Computer Engineer post-production.*
