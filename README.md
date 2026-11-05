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
- Quote funnel: each completed request is emailed to tmcmanuspowerup@gmail.com through FormSubmit (`LEAD_EMAIL_ENDPOINT` near the top of the script in `index.html`). The very first submission triggers a one-time activation email to that inbox; click "Activate Form" or no leads are delivered.
- If the email can't be sent, the visitor gets a text-message and call fallback to the Rocklin office, (916) 350-1417 (`LEAD_SMS`).
- Careers, Dealer and Referral forms still use the text-message handoff.
