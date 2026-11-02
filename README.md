# Power Up Solutions — site revamp

Live: https://jamesonflex.github.io/Power-Up-Solutions/

Static one-page site (no build step). GitHub Pages serves `main` from the repo root.

## Files
- `index.html` — whole site (pages switch by `#hash`)
- `img/` — photos, logo (white/black), icons, `share-preview.jpg` (1200x630 link preview)
- `favicon.ico`, `apple-touch-icon.png`, `site.webmanifest` — tab / home-screen icons
- `robots.txt`, `sitemap.xml`

## Moving to a custom domain
Find-and-replace `https://jamesonflex.github.io/Power-Up-Solutions/` in `index.html`, `robots.txt` and `sitemap.xml` with the new domain, then add a `CNAME` file.

## Lead routing
Forms currently hand off by text message to (916) 824-4650 (`LEAD_SMS` near the top of the script in `index.html`). Connect to a CRM webhook before running paid traffic.
