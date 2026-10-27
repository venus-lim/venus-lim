# EcoGlobal Sales & Lead CRM Portal (`ecoglobal-sales-portal`)

**Company:** EcoGlobal Development Corp.  
**Repository Visibility:** Private (`423` files · `61` commits · 12-folder `docs/` tree)  
**Connected Public Website:** [https://condormitel.homes](https://condormitel.homes)

---

### 1. System Purpose
An internal property sales CRM and inquiry tracking dashboard combined with the public lead-generation landing page (**[condormitel.homes](https://condormitel.homes)**). Designed to capture prospective student housing and unit inquiries from web forms and Meta ad campaigns and route them directly into staff follow-up queues.

---

### 2. Core Workflow & Platform Integrations
* **Lead Capture (`condormitel.homes` & `meta-leads-webhook`):**
  * Custom domain configured via **GoDaddy DNS** and connected to an automated webhook listener (`meta-leads-webhook`) that captures Facebook/Meta lead form submissions and website inquiries in real time.
* **CRM Pipeline & Follow-Up:**
  * Centralizes inquiry statuses, showroom visit scheduling, and reservation handoffs so leasing staff have a single view of incoming prospects.
* **Cloud & Service Stack:**
  * **Supabase:** Cloud PostgreSQL database for lead and sales records.
  * **Render:** Backend API hosting and **Render Static Sites** deployment.
  * **Brevo:** Automated confirmation and follow-up email delivery.
  * **Doppler:** Centralized environment variable management across development and production environments.
