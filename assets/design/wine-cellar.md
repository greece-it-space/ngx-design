# Wine Cellar Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Wine bars, enotecas, sommelier-led restaurants, tasting rooms, and hotel wine cellars.

## Visual Direction

Candlelit, scholarly, and warm. The page should feel like descending into a vaulted cellar at dusk: deep burgundy walls, parchment menus, brass candlelight, and reverence for the list. Wine forward, never showy.

## Theme Mode

- **Primary mode:** dark
- **Why:** the cellar metaphor only works on a deep burgundy/charcoal surface. Candlelight gold and parchment are accent values that depend on dark backgrounds to glow.
- **How to apply in the consuming project:**
  - Default `data-mode` to `'dark'` in `src/index.html`, persist `'dark'` in `localStorage` for `app-mode`.
  - Tune `html[data-mode='dark']` in `src/styles/_theme.scss` to the Palette below.
  - Tune `:root` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#1A0D14` (burgundy night)
- `--c-bg-secondary`: `#2B1620`
- `--c-bg-tertiary`: `#3A1E2A`
- `--c-text-strong`: `#F4E8D2` (parchment)
- `--c-text`: `#D4C5AB`
- `--c-text-muted`: `#8A7C6A`
- `--c-primary`: `#E8B86C` (candlelight gold — primary accent)
- `--c-secondary`: `#6B2C3A` (mulled wine — secondary accent)
- `--c-border`: `#3A2530`
- `--shadow-md`: `0 10px 30px rgba(0, 0, 0, 0.55)`
- `--focus-ring`: `0 0 0 3px rgba(232, 184, 108, 0.40)`

## Secondary Mode Fallback

Light mode should read as a daylit tasting room: `--c-bg-primary` `#F6EDDC`, `--c-bg-secondary` `#FFF8E8`, `--c-text-strong` `#1A0D14`, `--c-text` `#3A1E2A`, `--c-border` `#D4C0A0`. Keep candlelight gold and mulled-wine accents at slightly lower saturation so they don't shout on a bright surface.

## Typography

- **Display:** `Cormorant Garamond` italic or `Playfair Display` for hero and section titles; tracking `+0.02em`.
- **Body:** `Crimson Text` or any quality book-serif at 16px, line-height 1.7.
- **Accents:** small caps for region labels ("PIEMONTE", "BURGUNDY") in gold.
- **Voice:** knowledgeable but inviting. Sommelier register: mention region, vintage, grape, mood — not marketing claims.

## Section Anatomy

- **Hero:** dark burgundy ground, candlelight-gold eyebrow ("Cellar since 1974"), serif italic display title, two-line lede, primary CTA ("Reserve A Table") + ghost link ("View The List").
- **The list:** stylized preview with 3–5 wine cards. Each card: region (small-caps gold), name (serif title), grape + vintage (body), short tasting note, price.
- **By the glass / flights:** horizontal row of flight cards with names like "Old World Reds" or "Champagne House Flight".
- **About the cellar:** paragraph on selection philosophy, sommelier name, and food pairing approach.
- **Visit:** address, opening hours (lean into evening), corkage policy line, reservation method.

## Avoid

- Stock imagery of grapes, barrels, or generic wine glasses unless treated very moodily.
- Wine-rating badges, scores, or shopping-cart UI patterns.
- Bright primary colors or playful illustrations.
- Long marketing claims ("award-winning", "best wine list"). Let the list speak.
