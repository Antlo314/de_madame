# De Madame — Official Site

Enterprise-grade single-page site for **De Madame** ([@de.madame.aye](https://www.instagram.com/de.madame.aye/)) — Haitian-American actress & recording artist. Dark editorial luxury: noir + champagne gold, high-contrast serif, restrained motion. Built from her real imagery (curated for elegance) with pure-CSS atmosphere.

## Preview locally
```bash
python -m http.server 8848
# then open http://127.0.0.1:8848
```
Or just open `index.html` in a browser.

## Deploy

**GitHub Pages** (this repo): Settings → Pages → Source = *Deploy from a branch* → `main` / `/ (root)` → Save. The site publishes at `https://antlo314.github.io/de_madame/`.

**Netlify / Vercel / Cloudflare Pages**: drag-and-drop this folder, or connect the repo. No build step — it's fully static.

## Structure
```
index.html          the site (self-contained: inline CSS + JS)
favicon.svg         gold "DM" monogram
site.webmanifest    PWA manifest
assets/site/        site-ready images + PNG/Apple icons
assets/instagram/   original source photos (archive)
README-HANDOFF.md   full client handoff + go-live checklist
BUILD-BRIEF.md      research & creative brief
```

## Before going live
See **[README-HANDOFF.md](README-HANDOFF.md)** for the full checklist. In short:
1. Set `BOOKING_EMAIL` in `index.html` (until then the booking form copies the enquiry and opens Instagram DM).
2. Add real Spotify/Apple links to the music cards (currently "soon").
3. **Confirm the "Wrong Address" film title & credit in writing** before adding any film/IMDb link or year — the credit is her own bio claim and is not yet verified.
4. Once the domain is live, fill the `canonical` / `og:url` / absolute `og:image` TODOs in `<head>`.

## Notes
Site passed a 26-fix adversarial QA pass (correctness, accessibility, responsive, brand/fact-check, completeness). No horizontal scroll at 320–1280px; WCAG AA touches throughout. No AI-generated likenesses — every photo is genuinely her.
