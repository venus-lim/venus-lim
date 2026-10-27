# Planet of the Capes — Collector Storefront & Catalog Showcase (`planet-of-the-capes-storefront`)

**Brand:** Planet of the Capes (*The Collector's Time Machine*)  
**Repository Visibility:** Private (`422` files · modular Node build pipeline)  
**Live Public Preview:** [https://planetofthecapes.shop](https://planetofthecapes.shop) *(Under Active Development)*

---

### 1. System Purpose
An interactive e-commerce storefront and digital catalog built for vintage and modern action figure collectors. Combines embedded short-form video reels with live catalog browsing, franchise filter tabs, and an interactive "Dibs" reservation preview.

*Development Note: The public storefront at [planetofthecapes.shop](https://planetofthecapes.shop) is live for preview while remaining site features and catalog tools continue under active development.*

---

### 2. Modular Build & Storefront Structure
```text
planet-of-the-capes-storefront/
├── CLAUDE.md          Operational rules, UI protocols & Cloudflare quota guardrails
├── sections/00–08     Modular HTML storefront sections edited independently
├── build.js           Node.js compiler assembling sections/ into standalone index.html
├── server.js          Local development preview server (http://localhost:3000)
├── scripts/           Pre-push verification (verify_safe_commit.js)
└── docs/ & context/   Brand context dossier, UI protocols & operational guides
```

* **Modular Section Compilation (`build.js`):** Instead of editing a single large HTML file, the storefront is split into isolated sections (`sections/00` through `08`) and compiled locally via `node build.js`.
* **Embedded Video Reels Showcase:** Mobile-responsive vertical video section displaying product reels directly inside the storefront.
* **Cloudflare Pages Quota Management:** Deployed via Cloudflare Pages with local pre-testing (`node server.js`) and grouped milestone pushes to stay within the 500 monthly build quota.
* **Pre-Push Sanitization (`scripts/verify_safe_commit.js`):** Automated check script that scans staged commits to prevent credentials, oversized media files (`>25MB`), or customer contact details from entering Git history.
