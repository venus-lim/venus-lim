# EcoGlobal Development Corp. — Systems Overview

**Engagement Scope:** 1-Year Contractual Development & Operations Span  
**Live Public Website:** [https://condormitel.homes](https://condormitel.homes)  
**Source Code Status:** Private (Contains internal operational workflows and property records)

---

### How the EcoGlobal Projects Fit Together

Across a one-year span serving 100+ dormers and 30 unit owners at **EcoGlobal Development Corp. / One Katipunan Residences**, work spanned three private repositories plus the public student housing inquiry website:

1. **[Workspace & Apps Script Console (`ecoglobal-workspace-automations`)](./workspace-apps-script-console.md)**
   * Contains the live daily Google Apps Script operations console (**Dormer Masterfile Central Code Module**, `v318 STAFF LIVE`) synced via `clasp`, as well as 49 pulled workspace scripts—including the public **[condormitel.homes](https://condormitel.homes)** inquiry site (`test-condormitel-homes-LIVE`), `meta-leads-webhook`, and `leads-reservations-live`.
2. **[Leasing Operations Dashboard (`ecoglobal-leasing-operations`)](./leasing-operations-platform.md)**
   * The standalone 11-hub web platform (`React`, `Vite`, `Express`, `Prisma`, `Supabase`) structured to receive the schema-aligned data from the Apps Script console.
3. **[Sales & Marketing CRM Portal (`ecoglobal-sales-portal`)](./sales-crm-and-lead-portal.md)**
   * A separate real-estate sales and marketing CRM monorepo (`client/`, `server/`, `database/prisma/`, `design-system/`) deployed on Render, Render Static Sites, and Supabase with secrets managed in Doppler.
