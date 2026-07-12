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

## ✅ Live links wired (research, July 2026)
| Platform | URL |
|---|---|
| Instagram | https://www.instagram.com/de.madame.aye/ |
| TikTok | https://www.tiktok.com/@de.madame.aye |
| *Wrong Address* on Tubi | https://tubitv.com/movies/100033521/wrong-address |
| Film Instagram | https://www.instagram.com/wrongaddressmovie/ |
| IMDb title page | https://www.imdb.com/title/tt35819880/ |

Film note: production materials (@wrongaddressmovie) bill her as **Avione Denoxolaux**. Site copy reflects that. Top-line IMDb cast lists are incomplete for smaller credits — IMDb link is the *title* page only, not a verified person credit.

## ⚠️ Still for client before / after go-live

1. **Booking email** — in `index.html`, find `const BOOKING_EMAIL="";`. Until set, the form copies the enquiry + opens Instagram DM.
2. **DSP streaming** — Spotify / Apple for "Texas Tippin" & "Let Me At Em" still show `· soon` (no public links found).
3. **Exact role name** on *Wrong Address* — optional polish once she confirms in writing.
4. **Domain / hosting** — unlocks canonical / `og:url` / absolute `og:image` TODOs in `<head>`.

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
