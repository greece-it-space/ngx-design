# Industrial Brewery Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Craft breweries, taprooms, gastropubs with in-house beer, beer halls, and brewery-restaurants.

## Visual Direction

Raw, industrial, honest. The page should feel like a working brewhouse: exposed concrete, iron, copper tanks, a chalkboard tap list, and zero marketing gloss. Function-first, beer-nerd-friendly.

## Theme Mode

- **Primary mode:** dark
- **Why:** the concrete/iron metaphor needs gray-on-dark to register; light mode collapses the industrial mood into a generic cafe look. Copper accent only glows on dark.
- **How to apply in the consuming project:**
  - Default `data-mode` to `'dark'`, persist `'dark'` in `localStorage` for `app-mode`.
  - Tune `html[data-mode='dark']` in `src/styles/_theme.scss` to the Palette below.
  - Tune `:root` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#1F1F1F` (iron black)
- `--c-bg-secondary`: `#2A2A2A` (concrete)
- `--c-bg-tertiary`: `#363636`
- `--c-text-strong`: `#ECE6D5` (oat malt)
- `--c-text`: `#C2BCA8`
- `--c-text-muted`: `#807A6E`
- `--c-primary`: `#B87333` (copper — primary accent)
- `--c-secondary`: `#D9A04E` (amber — secondary accent)
- `--c-border`: `#383838`
- `--shadow-md`: `0 6px 18px rgba(0, 0, 0, 0.45)`
- `--focus-ring`: `0 0 0 3px rgba(184, 115, 51, 0.40)`

## Secondary Mode Fallback

Light mode should feel like a daytime taproom: `--c-bg-primary` `#EDEAE2`, `--c-bg-secondary` `#FBF9F2`, `--c-text-strong` `#1F1F1F`, `--c-text` `#383838`, `--c-border` `#CFCBBE`. Keep copper and amber accents identical — they work across modes.

## Typography

- **Display:** `Bebas Neue`, `Anton`, or `Oswald`. Heavy condensed sans, uppercase.
- **Body:** `Inter` or system sans, 16px, line-height 1.55.
- **Accents:** `JetBrains Mono` or any monospace for ABV, IBU, OG/FG, tap numbers, tasting notes.
- **Voice:** beer-nerd honest. Use real specs (ABV, IBU, hops, yeast, malt). No empty descriptors like "smooth" or "refreshing".

## Section Anatomy

- **Hero:** iron-black ground, copper eyebrow ("Brewing on-site since 2018"), condensed uppercase display title, 1-line lede, primary CTA ("View Tap List") + ghost link ("Visit the Brewhouse").
- **Tap list:** dense table or tight grid. Each row/card: tap number (mono), beer name (display), style, ABV / IBU (mono), 1-line tasting note, price for pour sizes.
- **The brewhouse:** short paragraph on equipment, head brewer, brewing philosophy. Avoid corporate language.
- **Food / kitchen** (if applicable): simple grid, no separate styling — same industrial language.
- **Visit:** address, hours, growler/crowler fill info, tours line, parking note.

## Avoid

- Decorative serifs, cursive, or "craft beer brand" calligraphy.
- Round, soft, watercolor labels — keep typography stencil/industrial.
- Stock imagery of generic clinking pints.
- Hiding tap-list specs behind hover/expand — keep ABV/IBU visible.
