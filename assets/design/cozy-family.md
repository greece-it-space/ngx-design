# Cozy Family Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Family restaurants, small cafes, casual dining places, guest houses, and local hotels.

## Visual Direction

Comfortable, warm, trustworthy, and easy to scan. The page should make families feel that the place is relaxed, practical, and welcoming — bright cream walls, golden yellow accents, coral-red highlights, chocolate-brown text.

## Theme Mode

- **Primary mode:** light
- **Why:** the warm cream/coral/yellow palette communicates daytime, family-friendly comfort. On dark it inverts to a moodier dinner setting that contradicts the brand promise.
- **How to apply in the consuming project:**
  - Set default `data-mode` to `'light'` in `src/index.html`, persist `'light'` to `localStorage` for `app-mode`.
  - Tune the `:root` block in `src/styles/_theme.scss` to the Palette below.
  - Tune `html[data-mode='dark']` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#FFF6E8` (warm cream)
- `--c-bg-secondary`: `#FFFBF2`
- `--c-bg-tertiary`: `#FBEFD8`
- `--c-text-strong`: `#8A5A3A` (chocolate brown)
- `--c-text`: `#5A4030`
- `--c-text-muted`: `#A38468`
- `--c-primary`: `#D86D4D` (coral red — primary accent)
- `--c-secondary`: `#F7C968` (golden yellow — secondary accent)
- `--c-border`: `#EAD8B8`
- `--shadow-md`: `0 8px 22px rgba(138, 90, 58, 0.12)`
- `--focus-ring`: `0 0 0 3px rgba(216, 109, 77, 0.40)`

## Secondary Mode Fallback

Dark mode should feel like the same room at dinner: `--c-bg-primary` `#2A1E14`, `--c-bg-secondary` `#3A2A1E`, `--c-text-strong` `#FFF6E8`, `--c-text` `#EAD8B8`, `--c-border` `#4A3624`. Keep coral and golden accents.

## Typography

- **Display:** `Lora` or `DM Serif Display`. Demo uses `Georgia`. Weight 600.
- **Body:** `Inter`, weight 400, line-height 1.65.
- **Voice:** plain, direct, family-warm. Mention kids' options, group seating, casual prices. No premium-restaurant register.

## Section Anatomy

- **Hero:** cream ground, coral eyebrow ("Family welcome since 1998"), serif display title, 2-line lede, primary CTA ("Reserve a Table") + ghost link ("View Menu").
- **Highlights:** kids' menu, group seating, everyday specials, comfort.
- **Menu preview:** simple categories, readable prices, no clutter.
- **Space/gallery:** seating, atmosphere, food. Lean into daylight.
- **About:** local trust, family ownership, neighbourhood ties.
- **Contact:** address, hours, phone, reservation, delivery info — all large and obvious on mobile.

## Avoid

- Premium fine-dining gloss, heavy effects, or dense copy.
- Hiding hours, phone, or address behind expand/click.
- Mood photography or dark interior shots.
- "Luxurious", "exclusive", "curated" — wrong register for this brand.
