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
- Quote funnel: each completed request is emailed through EmailJS (service_vg0buu1 / template_4okl5ze, sent from Jameson's Gmail to tmcmanuspowerup@gmail.com, Bcc solarjameson@gmail.com). Settings live in the `EMAILJS` constant near the top of the script in `index.html`. Free plan: 200 emails/month.
- If the email can't be sent, the visitor gets a text-message and call fallback to the Rocklin office, (916) 350-1417 (`LEAD_SMS`).
- Careers, Dealer and Referral forms still use the text-message handoff.
