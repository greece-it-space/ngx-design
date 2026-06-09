# Luxury Dark Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Exclusive restaurants, high-end lounges, private clubs, luxury hotel venues, and premium hospitality programs.

## Visual Direction

Dramatic, dark, exclusive, precise, and elegant. The page should feel premium without becoming hard to read — true black surfaces, rich gold and champagne accents, ivory text, generous space, and strong hierarchy.

## Theme Mode

- **Primary mode:** dark
- **Why:** this is the catalog's only true dark-native design. Gold and champagne accents only register as luxury against black; on a light surface they flatten into generic brand colors and lose the exclusivity.
- **How to apply in the consuming project:**
  - Set `document.documentElement.setAttribute('data-mode', 'dark')` as the default in `src/index.html` and persist `'dark'` to `localStorage` for `app-mode`.
  - Tune the `html[data-mode='dark']` block in `src/styles/_theme.scss` to the Palette below.
  - Tune the `:root` (light fallback) block to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#0F0F0F` (jet black)
- `--c-bg-secondary`: `#1A1A1A`
- `--c-bg-tertiary`: `#2A2A2A`
- `--c-text-strong`: `#F5F1EB` (ivory)
- `--c-text`: `#D6D0C2`
- `--c-text-muted`: `#A39D7F` (muted gold)
- `--c-primary`: `#D4AF37` (rich gold — primary accent)
- `--c-secondary`: `#F4D4A8` (champagne — secondary accent)
- `--c-border`: `#2D2D2D`
- `--shadow-md`: `0 12px 30px rgba(0, 0, 0, 0.55)`
- `--focus-ring`: `0 0 0 3px rgba(212, 175, 55, 0.45)`

## Secondary Mode Fallback

Light mode reads as the same brand printed on premium card stock: `--c-bg-primary` `#FAF7F0`, `--c-bg-secondary` `#FFFFFF`, `--c-text-strong` `#0F0F0F`, `--c-text` `#2A2A2A`, `--c-border` `#E4DDC6`. Keep gold and champagne accents at slightly lower saturation so they don't shout on a bright surface.

## Typography

- **Display:** `Cormorant Garamond` or `Playfair Display`. Demo uses `Georgia`. Weight 500–700.
- **Body:** `Lora` or `Crimson Text`, weight 400, line-height 1.7.
- **Voice:** confident and restrained. Service, access, menu, reservation details — make exclusivity concrete, not abstract.

## Section Anatomy

- **Hero:** jet ground, gold eyebrow ("Exclusive luxury"), serif display title, two-line lede, primary CTA ("Request Access") + ghost link ("Discover Our Venues").
- **Experiences:** fine dining, luxury rooms, private lounge — each as a richly described card with specific service detail.
- **Menu / drinks / membership preview:** small named selection with brief notes and pricing band.
- **Gallery:** strong-contrast premium detail shots — private dining room, suite, lounge, cocktail.
- **Private event / exclusive service:** concierge-style section with response time and contact channel.
- **Reservation / contact:** reservation method, location, hours, policies (dress code, minimum spend if applicable).

## Avoid

- Sacrificing accessibility for atmosphere. Dark UI still needs WCAG AA contrast and visible focus states.
- Bright neon or saturated brand colors — luxury here is gold-on-black, not pink-on-black.
- Casual or friendly copy. This brand sells discretion.
- Loyalty-program prompts or popups — wrong register entirely.
