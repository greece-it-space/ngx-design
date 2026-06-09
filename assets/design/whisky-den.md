# Whisky Den Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Whisky bars, cigar lounges, hotel cigar rooms, members-only nightcap venues, and gentlemen's club-styled bars.

## Visual Direction

Discreet, members-only, late-hour. The page should feel like the back room of a country hotel at 11pm: tobacco-brown walls, oxblood leather chairs, tarnished brass lamps, decanters of single-malt, hushed voices. Not flashy luxury — quiet authority.

## Theme Mode

- **Primary mode:** dark
- **Why:** the nightcap-room metaphor only works on warm brown/oxblood backgrounds. The tarnished brass accent is intentionally muted — it loses identity on a white surface.
- **How to apply in the consuming project:**
  - Default `data-mode` to `'dark'`, persist `'dark'` in `localStorage` for `app-mode`.
  - Tune `html[data-mode='dark']` in `src/styles/_theme.scss` to the Palette below.
  - Tune `:root` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#2A1810` (tobacco)
- `--c-bg-secondary`: `#3A2418`
- `--c-bg-tertiary`: `#4A2E20`
- `--c-text-strong`: `#F0E5C8` (parchment cream)
- `--c-text`: `#C8B89A`
- `--c-text-muted`: `#847465`
- `--c-primary`: `#9C7A3B` (tarnished brass — primary accent)
- `--c-secondary`: `#5A1A1A` (oxblood — secondary accent)
- `--c-border`: `#432B1F`
- `--shadow-md`: `0 10px 30px rgba(0, 0, 0, 0.5)`
- `--focus-ring`: `0 0 0 3px rgba(156, 122, 59, 0.40)`

## Secondary Mode Fallback

Light mode reads as a daylit club library: `--c-bg-primary` `#F2E6CC`, `--c-bg-secondary` `#FBF4E2`, `--c-text-strong` `#2A1810`, `--c-text` `#4A2E20`, `--c-border` `#D9C29A`. Keep brass and oxblood accents.

## Typography

- **Display:** `Cinzel` or `Cormorant SC` (small-caps serif), weight 500–600. Club-emblem energy.
- **Body:** `Lora` or `Crimson Text`, weight 400, line-height 1.7.
- **Accents:** small caps and numerals for vintage years ("18 YEARS", "1972 BOTTLING").
- **Voice:** discreet. Distillery, region, age, cask. No "best", no "world-class". Let the bottle list speak.

## Section Anatomy

- **Hero:** tobacco ground, brass eyebrow ("Members & invited guests"), small-caps display title, 2-line lede, primary CTA ("Reserve The Library") + ghost link ("Tonight's Pour").
- **The library / bottle list:** preview of the collection. Each card: distillery (display small caps), region (eyebrow), age, cask type, brief tasting note, pour price.
- **Cigars / pairing** (optional): small grid of cigar offerings if applicable, with origin and pairing suggestions.
- **The room:** quiet paragraph on policy, dress code, membership/guest access.
- **Reserve / visit:** address, hours (late evening), reservation method, members access note.

## Avoid

- Loud "luxury" gold-on-black gloss. This is restrained, not aspirational.
- Stock cigar/whisky photos with shallow depth-of-field clichés.
- Marketing claims about award-winning bottles. Cite age and cask, let it stand.
- Family-friendly framing. The audience is adult, evening-only.
