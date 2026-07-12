# DE MADAME — Official Site Build Brief
> Handoff doc. Research + assets complete. Next session (Opus): build the site from this brief.

## 1. Who she is (verified from Instagram @de.madame.aye, July 2026)
- **Name/brand:** De Madame (De Madame Aye)
- **Followers:** 102K on Instagram · 13 posts · 1,238 following
- **Bio (verbatim):** "Aries ♈️ Femme Fatale | LaMamiWata 🧜🏽‍♀️ / Actress | Artist 🇭🇹 Haitian With No Patience / Movie 🎥 'Wrong Address' 🔮 mwen bèl. Belle Âme"
- **Identity:** Haitian-American actress, recording artist, content creator. Works between **Dallas, TX and Mississippi**.
- **Music:** songs **"Texas Tippin"** (performed live at car shows) and **"Let Me At Em"** (has BTS shoot content).
- **Film:** appears in **"Wrong Address"** — likely [Wrong Address (2025), IMDb tt35819880] — CONFIRM with client before publishing.
- **Signature phrases (use as pull-quotes):**
  - "I don't compete for a spot, I am the spot."
  - "Mwen bèl. Belle Âme." (Haitian Creole: "I am beautiful. Beautiful soul.")
  - "Carrying myself like the investment I am."
  - "Haitian With No Patience"
- **Motifs:** LaMamiWata (Haitian/African water-spirit — mermaid, water, gold), Aries, femme fatale, mirrors, Creole heritage.
- No external link-in-bio, TikTok/Spotify/YouTube presence found via search. Ask client for streaming/booking links.

## 2. Brand direction — "Elegant yet sensual"
- **Tone:** magnetic confidence, editorial luxury, Vogue-cover not club-flyer. Sensuality through poise, silhouette, and gaze — never explicit.
- **Palette:** deep noir (#0B0A0D), champagne gold (#D4AF7A), warm ivory (#F5EFE6), accent oxblood (#5C1A1A) or deep teal (#0E3B3B, Mami Wata water). Dark theme primary.
- **Type:** high-contrast serif display (Playfair Display / Cormorant Garamond) + clean grotesque body (Inter / Neue Montreal style). Generous letterspacing on caps for labels.
- **Texture:** subtle water caustics / silk motion in hero, gold hairline rules, film-grain overlay on photos.

## 3. Site structure (single-page + press kit, enterprise grade)
1. **Hero** — full-bleed portrait (upscaled `spot-hero.jpg` or AI cinematic video loop), name in large serif, tagline: "Actress. Artist. Femme Fatale." CTA: "Bookings & Press".
2. **About / La Madame** — bio narrative weaving Haitian heritage, Creole quotes with translations, Aries/Mami Wata mythology as brand story.
3. **Film** — "Wrong Address" feature card (poster placeholder → AI prompt below), role, year, link.
4. **Music** — "Texas Tippin" + "Let Me At Em" cards with streaming links (get from client) and live-performance photo.
5. **Gallery** — masonry editorial grid from assets folder (hover: caption quotes). Tasteful selection only.
6. **Press / Media Kit** — stats (102K IG), downloadable EPK, high-res headshots.
7. **Bookings / Contact** — form or mailto for bookings, appearances, collabs, press. Instagram DM link.
8. Footer — socials, © De Madame 2026.
- Responsive, dark, smooth-scroll, subtle parallax; keep animations restrained (fade/translate only).

## 4. Downloaded assets (`assets/instagram/`, 640px — upscale to 2K via Higgsfield upscale_image before hero use)
| file | content / caption source | use |
|---|---|---|
| spot-hero.jpg | "I don't compete for a spot, I am the spot" | Hero / About |
| mirror-confidence.jpg | Mirror, confidence post | Gallery |
| texas-tippin-performance.jpg | Car-show performance of "Texas Tippin" | Music section |
| bts-let-me-at-em.jpg | BTS "Let Me At Em", Dallas/Mississippi | Music/Gallery |
| belle-ame-elegance.jpg | "Carrying myself like the investment I am 🩰🤍 Belle Âme" | About / Gallery (classiest) |
| let-me-at-em-promo.jpg | "Let Me At Em" promo | Music |
| profile-pic.jpg | avatar (150px only) | favicon/schema only |

Deliberately excluded 2 provocative posts per client direction. CDN URLs are signed/expiring — files are saved locally, don't hotlink.

## 5. AI generation prompts (Higgsfield — generate_image / generate_video)
**Hero video loop (5–8s, 16:9):** "Cinematic slow-motion portrait of an elegant Haitian woman in a flowing champagne-gold silk gown, standing in dark water reflecting golden light, gentle ripples, mermaid-goddess Mami Wata aesthetic, editorial fashion film lighting, deep noir background, subtle film grain, luxurious, poised, sensual but tasteful, camera slowly pushes in."
**About backdrop (image, 16:9):** "Abstract dark editorial backdrop, deep black silk fabric with golden water caustics light patterns, oxblood and champagne accents, luxury perfume-campaign aesthetic, no people, high detail."
**Film section poster placeholder (2:3):** "Moody drama film poster style photograph, city doorway at dusk, warm tungsten light spilling out, mysterious elegant silhouette of a woman in a long coat, film noir, no text."
**Music section visual (1:1):** "Luxury single cover art: gold vinyl record dissolving into water ripples on black背景 — replace with: black background, champagne-gold typography space, elegant, minimal."
**Section divider (video 3s, subtle):** "Slow gold ink swirling in dark water, macro, elegant, seamless loop, black background."
**Photo treatment note:** upscale all IG photos ×2 (upscale_image), optional remove_background on spot-hero for layered hero composition.

## 6. Open questions for client
1. Streaming links (Spotify/Apple) for the two songs? 2. Confirm "Wrong Address" IMDb credit + role name. 3. Booking email address. 4. TikTok/YouTube handles if any. 5. Domain name preference.

## 7. Build instructions for next session
- Build as static single-page site in this folder (`index.html` + `assets/`), or via Higgsfield `create_website` if user wants hosted deploy — ask which.
- Preview with the in-app browser; verify mobile (375px) and desktop.
- Use assets from `assets/instagram/`; run Higgsfield upscale on spot-hero + belle-ame first.
