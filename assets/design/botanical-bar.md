# Botanical Bar Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Plant-forward cocktail bars, greenhouse-themed bars, garden restaurants at night, botanical cocktail rooms, and gin-and-herb-led venues.

## Visual Direction

A greenhouse after dark. The page should feel like a glass conservatory at 10pm: deep forest walls, hanging foliage in silhouette, brass lamp glow, terracotta pots, cream linen napkins. Plants set the mood, cocktails are the medium.

## Theme Mode

- **Primary mode:** dark
- **Why:** the night-greenhouse metaphor is the whole point. Light mode collapses the after-dark conservatory feel into a generic plant-shop look. Forest green only registers as a room (not a brand color) on a dark surface.
- **How to apply in the consuming project:**
  - Default `data-mode` to `'dark'`, persist `'dark'` in `localStorage` for `app-mode`.
  - Tune `html[data-mode='dark']` in `src/styles/_theme.scss` to the Palette below.
  - Tune `:root` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#0F2A1E` (deep forest)
- `--c-bg-secondary`: `#173A29`
- `--c-bg-tertiary`: `#1F4533`
- `--c-text-strong`: `#F2EAD3` (linen cream)
- `--c-text`: `#C4B898`
- `--c-text-muted`: `#7C7560`
- `--c-primary`: `#B89968` (brass — primary accent)
- `--c-secondary`: `#C97A4A` (terracotta — secondary accent)
- `--c-border`: `#1F4533`
- `--shadow-md`: `0 10px 30px rgba(0, 0, 0, 0.5)`
- `--focus-ring`: `0 0 0 3px rgba(184, 153, 104, 0.40)`

## Secondary Mode Fallback

Light mode reads as a daylit conservatory: `--c-bg-primary` `#EFEADA`, `--c-bg-secondary` `#FBF6E8`, `--c-text-strong` `#0F2A1E`, `--c-text` `#1F4533`, `--c-border` `#D2C9AE`. Keep brass and terracotta accents.

## Typography

- **Display:** `Fraunces` or `Playfair Display`, italics welcome for botanical names.
- **Body:** `Inter`, weight 400, line-height 1.65.
- **Accents:** italic latin botanical names ("Cynara scolymus"), small caps for herb labels.
- **Voice:** plant-literate, sensorial. Mention herbs, ferments, infusions, foraged ingredients. Specific, never vague.

## Section Anatomy

- **Hero:** deep-forest ground, brass eyebrow ("Botanical cocktail room"), serif italic display title, 2-line lede, primary CTA ("Reserve a Table") + ghost link ("Tonight's Menu").
- **The garden / cocktail menu:** 3–4 signature cocktails. Each card: cocktail name (display), botanical ingredient list (latin italics + common name), brief flavor note, price.
- **In the greenhouse:** paragraph on growing program, foraging partners, fermentation lab.
- **Pair / bites** (optional): plant-forward small plates if served.
- **Visit:** address, hours, reservation method, garden tour info if applicable.

## Avoid

- Tropical / beach / summer-festival imagery.
- Bright daylight greenhouse photos — lean into night and lamp glow.
- Cliched leaf-pattern backgrounds. Use real plant photography or none.
- Wellness/yoga voice. This is a bar, not a wellness retreat.
