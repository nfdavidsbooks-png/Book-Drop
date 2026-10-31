# Book Drop - PWA starter

This is the first runnable, installable-phone-app foundation for Book Drop.

## Included
- Responsive mobile-first interface
- Six selectable themes
- Discovery inbox that saves shared URLs locally
- Manual book entry
- TBR, currently reading, read, DNF, owned and wishlist shelves
- Audiobook shelf and series grouping
- Local persistence using browser localStorage
- PWA manifest, service worker and app icon

## Important current limitations
This is a front-end starter, not a deployed production service. It does not yet have accounts, cloud sync, AI extraction from social videos, live book metadata, ISBN matching, retailer inventory, price comparisons or verified audiobook availability. The format checkboxes are user-entered notes, not retailer verification.

## Run locally
A service worker and install prompt require localhost or HTTPS. From this folder, run:

    python -m http.server 8000

Then open:

    http://localhost:8000

For Android installation, deploy the folder to an HTTPS host, open it in Chrome, then use the browser menu's "Install app" or "Add to Home screen" option.

## Recommended next production steps
1. Choose hosting and a backend (for example Supabase for authentication and Postgres).
2. Add a secure server-side book metadata service using licensed/appropriate book data providers.
3. Implement a social-link ingestion pipeline that respects each platform's API and terms.
4. Add retailer/affiliate feeds and region-aware availability checks.
5. Add cloud sync, backups, privacy controls, accessibility checks and automated tests.
