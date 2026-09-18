# Merchants List — Landing Page

Static HTML site for **Merchants List**, a verified database of 2,238 U.S. dropshipping and Amazon FBA suppliers.

No build step, no dependencies — plain HTML/CSS/JS.

## Pages

- `index.html` — home / landing
- `blog.html` — 2026 U.S. supplier research report (SEO)
- `compare.html` — SaleHoo vs Worldwide Brands vs Merchants List
- `*-suppliers.html` — 8 industry pages (retail, wholesale, food, beauty, sports, electronics, apparel, pet)

## Run locally

Serve the folder (paths are absolute from root, so serve the folder itself):

```bash
python3 -m http.server 8000
# then open http://127.0.0.1:8000/
```

## Deploy

Live at **https://merchants.ai2eo.com/** (Vercel, auto-deploy from `main`).

- **Vercel** — `vercel.json` sets `cleanUrls:true, trailingSlash:false`.
  All asset/page links are absolute-from-root (`/assets/...`, `/retail-suppliers.html`)
  so pages keep working under clean URLs (`/retail-suppliers/`).
- **Netlify** — drag-and-drop the file, or connect the repo
- **GitHub Pages** — Settings → Pages → deploy from branch

## Before going live

Already done (Aug 2026), kept here for reference:

- [x] All `href="#"` buy buttons → real Gumroad checkout URLs
- [x] Footer contact email → `info@ai2eo.com`
- [x] Canonical/OG/sitemap → `https://merchants.ai2eo.com/`
- [ ] Confirm the verification date ("July 2026") still matches the current data file if you update `merchants_enriched.csv` later

## Stack

Plain HTML/CSS/JS. Fonts: Big Shoulders Display, IBM Plex Mono, IBM Plex Sans (Google Fonts).
