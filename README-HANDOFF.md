# De Madame — Official Site · Handoff

An enterprise-grade single-page site for **De Madame** (@de.madame.aye). Dark editorial luxury — noir + champagne gold, high-contrast serif, restrained motion. Built from her real Instagram assets (curated for class) + pure-CSS atmosphere. **No AI-generated likenesses** — every photo is genuinely her.

## Files
```
index.html                 ← the site (self-contained: inline CSS + JS)
favicon.svg                ← gold "DM" monogram
assets/site/               ← processed, site-ready images (cropped, graded, sharpened)
assets/instagram/          ← original downloads (archive)
BUILD-BRIEF.md             ← research + creative brief
```

## Run / preview locally
Open a terminal in this folder and run:
```
python -m http.server 8848
```
Then visit `http://127.0.0.1:8848`. (Open `index.html` directly via `file://` works in most browsers too.)

## ⚠️ Placeholders to fill before going live
These are intentionally left for the client — all clearly marked in code:

1. **Booking email** — in `index.html`, find `const BOOKING_EMAIL="";` (in the `<script>`). Set it to the real address, e.g. `"bookings@demadame.com"`. Until set, the booking form **copies the enquiry to the clipboard and opens her Instagram DM** (no lead is lost, no bouncing mail), and the "Bookings" contact link points to Instagram. Once you set the email, the form switches to opening the visitor's mail app pre-filled.
2. **Streaming links** — the "Texas Tippin" / "Let Me At Em" cards show `Spotify · soon` / `Apple · soon` chips (disabled). When DSP links exist, replace those `<span class="chip soon">` with `<a class="chip live" href="…" target="_blank" rel="noopener">`.
3. **"Wrong Address" film — IMPORTANT** — the film name comes from her own Instagram bio, so it's presented as her stated work, but the copy claims **no specific role and no year**, and the live IMDb link was **removed**. A fact-check found the IMDb title `tt35819880` ("Wrong Address," 2025) is a real Dallas drama whose listed cast does **not** appear to include her — so it may be a different film or an uncredited part. **Do not add an IMDb/streaming link or a year until she confirms the exact title and her credit in writing.** When confirmed, restore a `<a class="link-gold" href="…">` in the Film section (replacing the "Full cast & credits — forthcoming" text) and add role/year to the meta-row.
4. **Domain / hosting** — see below. The domain also unlocks three SEO/social items currently left as commented TODOs in `<head>`: `<link rel="canonical">`, `og:url`, and switching `og:image` to an absolute URL (relative image URLs don't render in Facebook/iMessage/LinkedIn link previews).

## Deploy options (pick one)
- **Netlify / Vercel / Cloudflare Pages (drag-and-drop):** upload this whole folder. Zero config — it's static.
- **GitHub Pages:** push the folder to a repo, enable Pages on the root.
- **Any web host:** upload `index.html`, `favicon.svg`, and the `assets/` folder, preserving structure.
- The site is fully static — no server or build step required.

## What's on the page
Hero · signature-quote marquee · stats · **La Madame** (bio + Haitian/Mami Wata story, Creole quote) · **Film** (Wrong Address) · **Music** (two singles) · studio pull-quote divider · **Gallery** · **Press / Media Kit** · **Bookings** form · footer. Fully responsive (mobile burger menu), accessible, dark-optimized, with JSON-LD `Person` schema for SEO.

## Quality pass
The page went through an adversarial multi-lens QA review (correctness, accessibility, responsive, brand/fact-check, completeness). 26 confirmed issues were fixed, including: the tablet-width nav break (768px iPad), the lead-losing booking form, WCAG items (skip link + `<main>` landmark, burger `aria-expanded`, focus-visible rings, 44px tap targets, `lang` tags on Creole/French, live-region form status), a fixed Creole-vs-French mislabel, softened factual claims about a real person, a full PNG/Apple/manifest icon set, and richer OG/Twitter/JSON-LD metadata. Verified: **no horizontal scroll at 320 / 375 / 768 / 1280px**, all images and fonts load, nav collapses correctly, menu + form interactions work.

> Note: the site renders best when you open it in your own browser — animations (reveal-on-scroll, marquee, gold shimmer) are paused in the embedded preview pane.

## Notes on the imagery
Only her most elegant frames were used prominently (white-turtleneck press shot, the "Belle Âme" portrait). Car-show/backside-heavy shots were deliberately excluded from hero/feature spots per the "class over provocative" direction. All photos carry a unifying noir+gold grade so snapshots read as a cohesive editorial set. Source images are 640px max (Instagram's public limit); if you can supply true high-res originals, drop them into `assets/site/` with the same filenames for crisper results.
