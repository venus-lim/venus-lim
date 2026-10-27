# Context Architecture & Modular Task Breakdown

This document outlines the standard repository structure and AI workflow used across my web, automation, and creative production projects.

---

## 1. Tri-Environment Claude & Antigravity Workflow

Rather than relying on unguided "vibe prompting," work is divided across specific environments and agent roles:

1. **Claude Native Desktop App (Connector Hub):**
   - Primary workspace when linking projects directly to external tools and extensions—connecting **Canva**, **Google Workspace**, the **Google Apps Script (`clasp`) extension**, and **CapCut**.
2. **VS Code Integration (File-by-File Curation):**
   - Used for hands-on project building where individual file edits are monitored directly, keeping folder structures aligned with UI sections (such as matching 11 sidebar sections to their corresponding folders) and maintaining consistent styling.
3. **Supervised Terminal CLI:**
   - Used under strict `CLAUDE.md` rules across isolated git worktrees for targeted verification tasks: running test scripts (`npm test`, `npm run verify`), checking folder and documentation alignment, running pre-push secret checks (`verify_safe_commit.js`), and syncing Google Apps Script files.
4. **Dividing Agent Responsibilities (`Claude` vs. `Google Antigravity`):**
   - To prevent agents from overwriting each other's work, **Claude** handles core application logic and database schemas, while **Google Antigravity** handles UI adjustments, documentation updates (`docs/`), and browser automation tasks.
5. **Task-Based Model Selection:**
   - Matches model capacity to task complexity—routing single-file edits to **Haiku**, standard feature work to **Sonnet**, and multi-file planning to **Opus** to keep token usage lean.

---

## 2. Obsidian Context Graphs & Modular Task Breakdown

* **Linked Documentation (`Obsidian` & `graphify`):**
  - Organizes project markdown files (`what`, `how`, `why`, `when`, `where`, `who`) into a linked map so the AI reads only the relevant rule files for a task instead of scanning the entire repository.
* **Defining Business Rules Up Front:**
  - Requires the AI to pause when a business rule is missing and clarify operational edge cases (such as blank fields, mid-month move-outs, or quota limits) before writing code.
* **Modular Task Breakdown:**
  - Large projects are broken down into smaller, self-contained task units with clear acceptance criteria and verification checklists—allowing the operator to stitch working components together with human QA rather than building monolithic systems in a single prompt.

---

## 3. Connected Cloud & Deployment Platforms

* **Supabase:** Cloud PostgreSQL database and file storage for contracts, receipts, and media assets.
* **Render:** Backend web service hosting and **Render Static Sites** for frontend deployment.
* **Cloudflare Pages:** Static storefront hosting and CDN delivery managed within the 500 monthly build quota via grouped milestone pushes.
* **Doppler:** Centralized environment variable and secret management so credentials never sit inside repository files.
* **Brevo:** Automated transactional email delivery using HTML templates.
* **GoDaddy:** Custom domain registration and DNS routing (`condormitel.homes`, `planetofthecapes.shop`).

---

## 4. Scope & Engineering Sign-Off

No claim is made to specialized Computer Science credentials. As the operator, I map the business workflows, organize the context architecture, and assemble the working modules—after which **every production codebase undergoes review and final sign-off by a Senior Licensed Computer Engineer post-production.**
