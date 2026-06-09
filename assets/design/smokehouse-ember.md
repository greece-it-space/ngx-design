# Smokehouse Ember Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Steakhouses, BBQ joints, grill houses, smoked-meat venues, and meat-forward gastropubs.

## Visual Direction

Smoke, fire, leather, and bronze. The page should feel like a low-lit grill room at service: charcoal walls, ember orange in the embers, leather banquettes, no apology for the carnivore agenda.

## Theme Mode

- **Primary mode:** dark
- **Why:** ember orange only reads as fire on a charcoal ground; on a bright surface it flattens to "construction safety orange". The smoke/leather mood requires darkness.
- **How to apply in the consuming project:**
  - Default `data-mode` to `'dark'`, persist `'dark'` in `localStorage` for `app-mode`.
  - Tune `html[data-mode='dark']` in `src/styles/_theme.scss` to the Palette below.
  - Tune `:root` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#1C1A18` (charcoal)
- `--c-bg-secondary`: `#2A2521`
- `--c-bg-tertiary`: `#3A332D`
- `--c-text-strong`: `#F4EBDA` (smoked cream)
- `--c-text`: `#C8B89E`
- `--c-text-muted`: `#847866`
- `--c-primary`: `#D9501E` (ember orange — primary accent)
- `--c-secondary`: `#8B5A2B` (leather brown — secondary accent)
- `--c-border`: `#3A332D`
- `--shadow-md`: `0 10px 30px rgba(0, 0, 0, 0.5)`
- `--focus-ring`: `0 0 0 3px rgba(217, 80, 30, 0.40)`

## Secondary Mode Fallback

Light mode should read as a daytime butcher counter: `--c-bg-primary` `#F2EBDC`, `--c-bg-secondary` `#FBF6EA`, `--c-text-strong` `#1C1A18`, `--c-text` `#3A332D`, `--c-border` `#D4C5A8`. Keep ember orange and leather accents — they map well to both modes.

## Typography

- **Display:** `Bebas Neue`, `Oswald`, or a slab serif like `Roboto Slab`. Heavy, condensed, uppercase for titles.
- **Body:** `Inter` or system sans. Weight 400, generous line-height.
- **Voice:** direct, confident, no-nonsense. Cuts of meat, weights, source farm, cook time. Don't apologize, don't oversell.

## Section Anatomy

- **Hero:** charcoal ground, ember-orange eyebrow ("Smoked in-house for 14 hours"), heavy uppercase display title, single-line lede, primary CTA ("Book a Table") + ghost link ("See The Cuts").
- **The cuts:** 3–4 card grid of signature dishes. Cut name (slab display), weight + source (mono body), 1-line description, price as ember accent.
- **Smoke + fire:** atmospheric paragraph about the pit, the wood, the dry-aging program — concrete details only.
- **Sides / sauces:** simple two-column list, leather-brown dividers.
- **Visit:** address, hours (lean into dinner), reservation method, walk-in policy.

## Avoid

- Pastels, floral motifs, or cozy/family copy.
- Vegetarian-forward hero imagery (sides can appear in a sub-section but don't lead with them).
- Cute mascots, cartoon flames, or playful illustrations.
- Listing every menu item — preview signature cuts, link to full PDF or sub-page for the rest.
