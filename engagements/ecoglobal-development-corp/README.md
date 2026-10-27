# EcoGlobal Development Corp. — Multi-System Operations Architecture

> **Engagement Scope:** 1-Year Contractual Development & Operations Span  
> **Live Public Property Portal:** [https://condormitel.homes](https://condormitel.homes)  
> **Source Code Status:** `🔒 Private` (Contains proprietary operational workflows and property records)

---

## System Ecosystem Overview

Three connected systems were built and maintained across a one-year span to support leasing, property management, and sales operations for **EcoGlobal Development Corp. / One Katipunan Residences** (serving 100+ dormers and 30 unit owners):

```text
[ condormitel.homes Public Website ]
               │
               ▼ (Meta Lead Webhooks & Inquiry Intake)
[ ecoglobal-sales-portal ] ──► [ ecoglobal-workspace-automations (v318 STAFF LIVE) ]
   (Sales & Lead CRM)             (Daily Google Workspace & Apps Script Console)
                                              │
                                              ▼ (Schema-Aligned Data Bridge)
                               [ ecoglobal-leasing-operations ]
                                  (11-Hub Full-Stack Platform)
```

---

## Public System Specifications in This Directory

1. **[Leasing Operations Platform (`ecoglobal-leasing-operations`)](./leasing-operations-platform.md)**
   - 11-hub property management and leasing platform built with React 19, Vite, Express 5, Prisma, and Supabase PostgreSQL.
2. **[Workspace & Apps Script Console (`ecoglobal-workspace-automations`)](./workspace-apps-script-console.md)**
   - Container-bound Google Apps Script operations console (`v318 STAFF LIVE`) synced via `clasp` CLI with local verification scripts (`npm run verify`).
3. **[Sales & Lead CRM Portal (`ecoglobal-sales-portal`)](./sales-crm-and-lead-portal.md)**
   - Internal property sales and lead tracking portal connected to `condormitel.homes`, Supabase, Render, Brevo, and Doppler.
