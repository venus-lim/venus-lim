# EcoGlobal Workspace & Apps Script Console (`ecoglobal-workspace-automations`)

> **Company:** EcoGlobal Development Corp. / One Katipunan Residences  
> **Repository Visibility:** `🔒 Private` (`1,699` files · `138` deployed console files · `319` reference docs)  
> **Production Deployment:** `v316–v318 STAFF LIVE` (Container-Bound Google Apps Script Web App)

---

## 1. System Purpose
Serves as the live daily operations console (**Dormer Masterfile Central Code Module**) used by staff to manage active tenancies, monthly ledgers, owner statements, utility schedules, and receipt intake while keeping every data write aligned with the target PostgreSQL schema in `ecoglobal-leasing-operations`.

---

## 2. Two-Tree `clasp` Mirror & Local Verification Workflow
Rather than editing scripts directly inside the browser-based Google Apps Script editor without version control, this repository maintains a local Git-tracked workflow:

```text
ecoglobal-workspace-automations/
├── CLAUDE.md                                   Root deployment rules & safety checks
├── src/apps-script/Apps Script Pulls/owned/    Live clasp deployment mirror (v318)
├── src/apps-script/Dormer Masterfile/console/  Local mock server (:8124) & test suite copy
├── console-tabs/                               Per-tab FEATURES.md specification ledger
├── tools/                                      Automated drift & reference verification scripts
└── references/                                 Deployment guides & schema alignment docs
```

---

## 3. Automated Quality & Deployment Guardrails
* **Pre-Push Verification (`npm run verify`):**
  * `tools/check_undefined_refs.js` — Checks that every function, menu item, and trigger referenced by the console is defined before deployment.
  * `tools/check_twins.js` — Ensures the local test mirror and the `clasp` deployment folder stay synchronized.
  * `npm run check:tabdocs` — Verifies that any code change to a sidebar tab includes a matching update to its `console-tabs/<tab>/FEATURES.md` documentation file.
* **Sensitive Data Protection:** Live dormer and owner spreadsheets (`live_data*.json`, `creds.json`, `token.json`) are strictly excluded via `.gitignore` so only clean application logic and documentation are committed to Git.
