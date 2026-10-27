# EcoGlobal Leasing Operations Platform (`ecoglobal-leasing-operations`)

**Company:** EcoGlobal Development Corp.  
**Repository Visibility:** Private (`1,241` files · `132` commits · `289` Markdown context docs)  
**Public Entry Point:** [https://condormitel.homes](https://condormitel.homes)

---

### 1. System Purpose
A centralized, multi-department property management and leasing operations dashboard designed to manage the lifecycle of residential units, property owners, tenants, utility billing, and lease contracts across four departments: **Leasing**, **PMO (Property Management Office)**, **Maintenance**, and **Accounting**.

---

### 2. Hub-Based Repository Structure (11 Operational Hubs)
Both the `/Frontend` (`React 19` + `Vite` + `Tailwind CSS`) and `/Backend` (`Express 5` + `Prisma` + `Supabase PostgreSQL`) mirror the 11 sidebar sections so every UI tab maps directly to its corresponding folder:

1. `property-assets` — Unit inventory, bed slot tracking, and key custody
2. `people-records` — Occupant, property owner, and staff record management
3. `leasing-lifecycle` — Inquiries, reservations, and lease contracts (`DRAFT` → `SIGNED` → `ACTIVE`)
4. `utility-billing` — Meter readings, utility proration, and Statements of Account
5. `rental-collections` — Monthly rent payment intake and deposit tracking
6. `owner-disbursements` — Owner payout schedules and disbursement records
7. `maintenance-inspections` — Work orders, unit inspections, and punchlists
8. `documents-vault` — Contract and receipt storage via Supabase Storage
9. `communications` — Automated email dispatch via Brevo HTML templates
10. `reports-analytics` — Occupancy and operational summary views
11. `system-administration` — Reference dictionaries, staff roles, and activity logs

---

### 3. Connected Infrastructure
* **Database & Storage:** Supabase (`PostgreSQL` + `Storage`) managed via `Prisma` schema migrations
* **Hosting:** Render (`Backend Web Service` + `Render Static Sites`)
* **Email Delivery:** Brevo transactional email templates
* **Environment Management:** Doppler secret management
* **Context Architecture:** `289` linked Markdown documentation files (`docs/what`, `docs/how`, `docs/why`, `docs/when`, `docs/where`, `docs/who`) governed by root `CLAUDE.md` rules and an isolated `/design-system` UI preview sandbox.
