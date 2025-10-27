# ComfortCare Reflexology

A simple, fast, **single‑page** static website for a massage spa. Bilingual (中文/EN), includes **services**, **pricing**, **booking (phone + email intent)**, **locations**, and **SEO tags**.

## Quick Edit

- Open `site.config.json` and update:
  - `"brand"` — your brand name
  - `"primary_email"` — where booking intent emails should go
  - `"locations"` — addresses, phones, hours, map links
  - `"services"` and `"addons"` — titles, durations, prices
  - `"social"` — Facebook/Instagram links

No build step is required. All content loads from `site.config.json` at runtime.

## Deploy (Pick One)

### Netlify (recommended for static sites)
1. Create a new site → **Deploy manually** → upload the folder.
2. Or drag‑and‑drop the folder to https://app.netlify.com/drop
3. Add a custom domain in **Domain management** and update your DNS A/AAAA/CNAME as instructed.

### Vercel
1. Create a new project → **Import** from Git or **Deploy** a static site.
2. Framework preset: **Other** (static).
3. Set `index.html` as the entry; no build command is needed.

### GitHub Pages
1. Create a repo and push the folder.
2. In **Settings → Pages**, set the branch to `main` (or `master`) and root folder `/`.
3. Wait for the publish URL.

## Custom Domain (DNS)
- Set a CNAME record for `www` to your hosting provider's subdomain (e.g., `cname.vercel-dns.com` or Netlify's target).
- Optionally set A/AAAA for apex `@` if your provider supports it (e.g., Netlify/Vercel provide IPs).
- Enable HTTPS in your provider's dashboard.

## Optional
- Replace `assets/favicon.svg` with your logo.
- Add Google Analytics 4 snippet in `<head>` if you need analytics.
- Add Yelp/Google review links to footer in `site.config.json > social`.

---

> This site uses **Tailwind via CDN**; for heavy traffic, consider a build pipeline later.
