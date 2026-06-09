# Cafe Bakery Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Coffee shops, bakeries, pastry venues, brunch cafes, and breakfast places.

## Visual Direction

Warm, friendly, bright, hand-made, and welcoming. The page should feel like a neighbourhood cafe at 9am: cream and tan walls, soft pink accents, the kind of polish that makes pastries look desirable without becoming corporate.

## Theme Mode

- **Primary mode:** light
- **Why:** the palette is built around cream and ivory backgrounds. Cafe-brown text and dusty-pink accents are designed to read on warm light surfaces; on dark they lose the bakery-window warmth.
- **How to apply in the consuming project:**
  - Set `document.documentElement.setAttribute('data-mode', 'light')` as the default in `src/index.html` and persist `'light'` to `localStorage` for `app-mode`.
  - Tune the `:root` block in `src/styles/_theme.scss` to the Palette below.
  - Tune the `html[data-mode='dark']` block to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#FAF8F5` (ivory)
- `--c-bg-secondary`: `#F5EDE3` (warm cream)
- `--c-bg-tertiary`: `#E8DCCF` (light tan)
- `--c-text-strong`: `#5A4A3A` (warm dark brown)
- `--c-text`: `#6B5344` (coffee brown)
- `--c-text-muted`: `#8B6F47` (cafe brown)
- `--c-primary`: `#8B6F47` (cafe brown — primary accent)
- `--c-secondary`: `#D4A5A5` (dusty pink — secondary accent)
- `--c-border`: `#D9C9BC`
- `--shadow-md`: `0 6px 18px rgba(107, 83, 68, 0.12)`
- `--focus-ring`: `0 0 0 3px rgba(212, 165, 165, 0.45)`

## Secondary Mode Fallback

Dark mode should read as the same cafe after hours: `--c-bg-primary` `#2A1F18`, `--c-bg-secondary` `#3A2A20`, `--c-text-strong` `#F5EDE3`, `--c-text` `#DCC9B6`, `--c-border` `#3D2A20`. Keep cafe-brown and dusty-pink accents — they translate well.

## Typography

- **Display:** `Inter` or `Fraunces` (warm serif). Demo uses `'Segoe UI'` system sans. Weight 600 for hero/H2, generous line-height.
- **Body:** `Inter`, weight 400, line-height 1.6.
- **Voice:** warm, friendly, local. Mention what's baked today, who makes it, opening time, weekend hours. Avoid corporate "premium coffee experience" language.

## Section Anatomy

- **Hero:** ivory ground, dusty-pink eyebrow ("Open from 7am"), warm display title, 2-line lede, primary CTA ("Order Online") + ghost link ("View Menu").
- **Signature products:** 3-card grid for coffee, pastries, breakfast plates, or seasonal specials. Card on warm cream ground, pink hairline accent, product name in brown, price as muted footnote.
- **Menu preview:** clear categories, real prices, no hidden information.
- **Gallery:** interior or product strip. Lean into morning light, never dark-and-moody.
- **About:** craft, freshness, local sourcing — concrete details only.
- **Contact:** hours, address, phone, order/reservation action.

## Avoid

- Dark photography, late-night atmosphere, or premium-restaurant gloss.
- Long marketing claims ("best coffee in town"). Mention origin, roaster, baker — let it speak.
- Dashboards, auth, CMS, API fetching, complex filtering, or heavy animation.
- Tiny mobile text. Keep hours/address/phone large and unmissable.
