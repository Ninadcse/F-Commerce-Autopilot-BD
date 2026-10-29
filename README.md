# F-Commerce Autopilot BD — Free Starter MVP

A mobile-friendly, no-build order register for Facebook, WhatsApp, Instagram and phone sellers in Bangladesh.

## Included
- Dashboard totals and recent orders
- Add/edit orders, customer phone/address, items, amount and advance paid
- Status tracking: Pending, Confirmed, Shipped, Delivered, Cancelled, Returned
- Customer directory built from order history
- Bangla message templates that you copy and send manually
- Search and filter, CSV export, JSON backup and restore
- Local browser storage and basic PWA/offline shell support
- No paid API, database, or build step required

## Run locally
Open `index.html` in a modern browser. Some PWA features require HTTPS, so use GitHub Pages for the installed-app/offline shell.

## Publish free with GitHub Pages
1. Create a public GitHub repository, e.g. `f-commerce-autopilot-bd`.
2. Upload `index.html`, `manifest.json`, `sw.js`, and this README to the repository root.
3. Open **Settings → Pages**.
4. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/(root)`, then Save.
5. Wait for GitHub Pages to publish. Your website URL will look like `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.
6. Open that HTTPS URL on your phone. Use the browser menu's **Add to Home screen** / **Install app** if available.

## Important limitations before charging customers
This is a working prototype, not yet a multi-user SaaS product. Orders are stored only in the current browser/device and can be lost if site data is cleared. There is no login, cloud sync, tenant separation, payment collection, automated Messenger/WhatsApp sending, or courier API integration. Do not promise these capabilities or store sensitive customer data at scale yet.

## Safe path to a paid business
1. Test with 3–5 sellers and gather feedback.
2. Define a clear paid plan and provide support.
3. Add Supabase authentication, database, row-level security and per-shop data isolation before using real customer accounts.
4. Add automated messages only through approved platform APIs, after confirming access and costs.
5. Add courier integrations and payment reconciliation only after validating which couriers and workflows customers actually use.
6. Publish privacy policy, terms, backup/export guidance, and a support contact before paid launch.

## Data safety
Export CSV for spreadsheets. Use **Reports & Export → Download backup JSON** for a full backup. JSON backups contain personal customer data; keep them secure.
