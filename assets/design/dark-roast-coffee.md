# Dark Roast Coffee Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Third-wave coffee roasters, evening coffee bars, dessert cafes, and roast-houses that pair coffee with cocktails or dessert.

## Visual Direction

Late-evening, roast-nerdy but warm. The page should feel like a roastery at 9pm: espresso-dark walls, copper portafilter glint, steamed-cream highlights, the smell of dark cocoa. The counterpart and counterpoint to the bright "Cafe Bakery" design.

## Theme Mode

- **Primary mode:** dark
- **Why:** espresso-brown surfaces, cream type, and copper accents are designed for evening. Light mode flattens the moody roastery atmosphere to a generic coffee shop.
- **How to apply in the consuming project:**
  - Default `data-mode` to `'dark'`, persist `'dark'` in `localStorage` for `app-mode`.
  - Tune `html[data-mode='dark']` in `src/styles/_theme.scss` to the Palette below.
  - Tune `:root` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#1F140E` (espresso)
- `--c-bg-secondary`: `#2D1F16`
- `--c-bg-tertiary`: `#3A2A1F`
- `--c-text-strong`: `#F0E2CC` (steamed cream)
- `--c-text`: `#C5B49A`
- `--c-text-muted`: `#847363`
- `--c-primary`: `#C28148` (copper — primary accent)
- `--c-secondary`: `#6B4A30` (cocoa — secondary accent)
- `--c-border`: `#3A2A1F`
- `--shadow-md`: `0 10px 30px rgba(0, 0, 0, 0.45)`
- `--focus-ring`: `0 0 0 3px rgba(194, 129, 72, 0.40)`

## Secondary Mode Fallback

Light mode reads as a morning roastery: `--c-bg-primary` `#F2E7D5`, `--c-bg-secondary` `#FBF4E5`, `--c-text-strong` `#1F140E`, `--c-text` `#3A2A1F`, `--c-border` `#D4C0A0`. Keep copper and cocoa accents.

## Typography

- **Display:** `Fraunces`, `Crimson Pro`, or similar high-contrast serif. Italics welcome for menu names.
- **Body:** `Inter` or `Sora`, weight 400, line-height 1.65.
- **Accents:** small caps for origin labels ("ETHIOPIA YIRGACHEFFE").
- **Voice:** roast-nerd warm. Mention origin, process, tasting notes, roast date. Avoid generic descriptors like "smooth" — be specific.

## Section Anatomy

- **Hero:** espresso ground, copper eyebrow ("Roasted weekly"), serif display title, 2-line lede, primary CTA ("Order Beans") + ghost link ("Tonight's Pour").
- **Today's roast / pour-over board:** 3–4 origin cards. Each card: origin (small-caps copper), process (washed/natural/honey), tasting notes (one line), price.
- **The roastery:** short paragraph on roaster, philosophy, sourcing. Mention specific producers if relevant.
- **Dessert / pairings** (optional): small grid if the venue serves dessert or cocktails.
- **Visit:** address, hours (lean into late opening for evening coffee bars), shop online link.

## Avoid

- Generic cafe-mug stock photos. Prefer roastery and brewing detail shots.
- Pastel "coffee with milk-foam art" hero — lean dark and moody.
- Vague tasting copy. Use third-wave specifics: variety, altitude, process.
- Family-friendly framing — this is for the third-wave / evening-coffee audience.
