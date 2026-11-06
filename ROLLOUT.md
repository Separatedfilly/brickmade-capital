# Brickmade Capital — rollout plan

## Recommended stack
- Static HTML/CSS in a GitHub repo → **Cloudflare Pages** (free, HTTPS automatic, preview URL per commit).
- No CMS, no forms, no build. Primary CTA is Email (`mailto:david.durgin@brickmadecapital.com` with subject “Discovery call — Brickmade Capital”). Phone deferred until a business number exists.
- Optional later: Calendly (if David prefers scheduling over mailto), Cloudflare Web Analytics (cookieless; update Privacy page if enabled), a contact form (Formspree / Cloudflare Pages Functions).

## Positioning locked for this draft
- Lead: CRE / real estate operations consulting.
- Secondary: AI productivity (also an add-on on CRE engagements).
- No rates, packages, or dollar amounts on the public site.
- Consulting-only; do not feature other ventures; do not claim Brickmade buys property.
- Careful with industrial acquisition language (non-compete geography from a prior operating role) — capital/underwriting support is framed as client-side advisory.

## Go-live steps (each requires David's explicit approval)
1. **Approve copy & design** of this v2 draft and fill the TODOs below. ← next decision
2. **Create GitHub repo** under David's account and push this folder.
3. **Create Cloudflare Pages project** linked to the repo (preset None, no build command, output `/`). Review the `*.pages.dev` preview.
4. **DNS change** — pick one:
   - A (simplest, least risk): keep DNS at GoDaddy; add `CNAME www → <project>.pages.dev` and redirect/forward apex to `www` (or use Cloudflare's instructions for the apex).
   - B (recommended long-term): move nameservers from GoDaddy to Cloudflare (domain registration stays at GoDaddy), then attach `brickmadecapital.com` + `www` in Pages.
   - Either way: **export current GoDaddy DNS first and recreate MX/TXT (SPF, DKIM, DMARC) records exactly** so david.durgin@brickmadecapital.com keeps working.
5. Verify HTTPS, mobile view, mailto links, 404 page; submit to Google Search Console (optional).

## Current GoDaddy "Launching Soon" page
- Leave it up until the Cloudflare preview is approved — it is harmless.
- At cutover, the DNS change in step 4 replaces it. Then turn off/cancel the GoDaddy Website Builder / parked page (and any paid GoDaddy site plan) so it doesn't conflict or keep billing. Do not cancel the domain registration or the email product.

## Open TODOs
- Optional headshot of David (`assets/dave.jpg`).
- Optional phone and/or LinkedIn URL on Contact.
- Optional Calendly (or similar) if mailto discovery CTA is not enough.
- Confirm public brand wording: site uses **Brickmade Capital**; bio source draft sometimes says **Brickmade Consulting** (practice under Brickmade Capital LLC).
- Confirm legal entity name "Brickmade Capital LLC" against the Certificate of Organization (footer, Privacy).
- Privacy "last updated" date; optional counsel review.
- Canonical URL / Open Graph image tags once the domain is live.
- Optional: hero/section photography from OneDrive `4. Consulting Website/2. Pictures/` (not used in this draft).
- Do **not** publish anything from the internal rate card on the website.

- Optional: add Call CTA once David has a business number.
