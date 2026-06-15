# pricer_web

Static marketing site for **Pricer** — the AI second-hand valuation app.

Plain HTML/CSS, no build step. Hosted free as a static site (GitHub Pages or
Cloudflare Pages) on **getpricerapp.com**.

## Files
- `index.html` — single-page landing
- `privacy.html` — Privacy Policy (copied from `pricer_legal`, kept in sync)
- `terms.html` — Terms of Use (copied from `pricer_legal`, kept in sync)
- `styles.css` — navy + gold brand system (mirrors the app's `src/theme/brand.ts`)
- `assets/` — badge + images

## Before launch — placeholders to replace
1. **App Store URL** — every `href="#download"` and the nav Download button.
   Expected: `https://apps.apple.com/app/id6774167590` (live once out of TestFlight).
2. **App Store badge** — `assets/app-store-badge.svg` is a placeholder. Swap for
   Apple's official badge (Apple marketing guidelines require the official art).
3. **App screenshots** — the hero phone mockup is CSS. Drop a real screenshot at
   `assets/screen-hero.png` and wire it into the `.hero-art` block.
4. **Reviews** — the `#reviews` section is built but `hidden`. No fake reviews
   (Authentic brand pillar). Unhide and fill with real App Store reviews once they exist.
5. **OG card** — add `assets/og-card.png` (1200×630) for social previews.

## Keep legal in sync
`privacy.html` / `terms.html` are the canonical legal copies in `pricer_legal`.
When they change there, re-copy them here.

## Deploy
Static host, no build. Point `getpricerapp.com` DNS at the chosen host
(GitHub Pages or Cloudflare Pages).

© 2026 Tobiassen Development
