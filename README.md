# The Beamish Society — Landing Page

The updated parent-corporation landing page. Single self-contained `index.html` (fonts from Google Fonts CDN, all CSS inlined, no build step).

## Deploy to Vercel

**Option A — drag & drop**
1. Go to [vercel.com/new](https://vercel.com/new)
2. Drag this `landing/` folder onto the page
3. Deploy. Done.

**Option B — Vercel CLI**
```bash
cd landing
vercel        # preview deploy
vercel --prod # production
```

**Option C — Git**
Push this folder to a repo and import it in Vercel. Set the **Root Directory** to `landing/` if the repo contains the whole design system. No framework preset needed — it's static HTML.

## Files
- `index.html` — the landing page (everything inlined; works offline except webfonts)
- `vercel.json` — clean URLs + sensible security headers

## Notes
- **Fonts** load from Google Fonts CDN (Pinyon Script + Cormorant Garamond). For fully self-hosted fonts, drop `.woff2` files alongside and swap the `<link>` for local `@font-face` rules.
- **Contact email** is `info@thebeamishsociety.com`. Confirm the TLD is correct (assumed `.com`); update the `mailto:` in `index.html` if not.
- **Copy** (tagline, the "instruments of trust" statement, the three principles, the enquiries note) is drafted in the Beamish voice — review and adjust before going live.
- Respects `prefers-reduced-motion`; reveals + the scroll cue disable for those users.
