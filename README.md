# Brickmade Capital — marketing site (v2 draft)

Plain HTML + one `site.css` + tiny `site.js` (mobile menu, footer year). No build step. All paths relative.

**Positioning (David-approved via Quartermaster, 2026-11-05):** lead with CRE / real estate operations consulting; AI productivity is a second service line and a CRE add-on. No rates or package prices on the site. CTA = Email to book (`mailto:david.durgin@brickmadecapital.com`). Phone CTA deferred until David establishes a business number. Consulting-only. No pricing copy on the site. Operator-depth bio lives on About only (not Home).

## Open locally
- Double-click `index.html`, or
- `python3 -m http.server 8000` in this folder, then open http://localhost:8000

## Files
- `index.html` Home · `about.html` Bio/About · `services.html` (CRE + AI) · `contact.html` · `privacy.html` · `404.html`
- `assets/brickmade-logo.png`, `assets/bm-icon.png`, `assets/favicon.png`, `assets/logo.svg` (from OneDrive `1. Logo`)
- Source copy: OneDrive `Documents/04 Brickmade Capital/7. Offerings/` — Services brief + Bio draft (2026-11-05). Internal rate card is **not** used on the site.
- Screenshots of the current draft: `/workspace/brickmade-capital-site-screens/`

## Remaining for go-live (all need David's approval)
1. Approve this v2 copy & design (fill remaining TODOs below / in HTML).
2. Create a GitHub repo (e.g. `brickmade-capital-site`, private OK) and push this folder — **do not create until David says so**.
3. Cloudflare Pages: connect the repo; framework preset "None", build command empty, output directory `/`.
4. Add custom domain `brickmadecapital.com` (+ `www`); update DNS at GoDaddy (or move nameservers to Cloudflare) — **do not change DNS until David says so**.
5. Preserve email (MX / SPF / DKIM / DMARC) for `david.durgin@brickmadecapital.com` during any DNS change.

See `ROLLOUT.md` for detail.
