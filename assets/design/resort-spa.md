# Resort Spa Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Wellness hotels, spa sanctuaries, nature retreats, and resort hospitality brands.

## Visual Direction

Calm, breathable, natural, and restorative. The page should reduce friction and communicate quiet, care, and escape — sage and teal greens, sky-blue softness, sand neutrals, natural light through every surface.

## Theme Mode

- **Primary mode:** light
- **Why:** the sage/teal/sand palette is built around daylight and natural materials. Dark mode breaks the "calm and breathable" promise that the brand is selling.
- **How to apply in the consuming project:**
  - Set default `data-mode` to `'light'` in `src/index.html`, persist `'light'` to `localStorage` for `app-mode`.
  - Tune the `:root` block in `src/styles/_theme.scss` to the Palette below.
  - Tune `html[data-mode='dark']` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#F4EFE3` (sand cream)
- `--c-bg-secondary`: `#FBF7EE`
- `--c-bg-tertiary`: `#E8DCC8` (sand)
- `--c-text-strong`: `#2D4A3A`
- `--c-text`: `#42584B`
- `--c-text-muted`: `#7E8E80`
- `--c-primary`: `#7FA88D` (sage — primary accent)
- `--c-secondary`: `#5A9B8A` (teal — secondary accent)
- `--c-border`: `#D4C9B2`
- `--shadow-md`: `0 12px 26px rgba(45, 74, 58, 0.10)`
- `--focus-ring`: `0 0 0 3px rgba(127, 168, 141, 0.45)`

## Secondary Mode Fallback

Dark mode for evening browsing (rare for this brand): `--c-bg-primary` `#1A2620`, `--c-bg-secondary` `#22322A`, `--c-text-strong` `#F4EFE3`, `--c-text` `#D4C9B2`, `--c-border` `#2D403A`. Keep sage and teal accents.

## Typography

- **Display:** `Fraunces`, `Lora`, or `Inter` display. Demo uses `'Segoe UI'`. Weight 500–600.
- **Body:** `Inter` or `Lora`, weight 400, line-height 1.7.
- **Voice:** gentle but concrete. List real treatments, packages, amenities, opening hours, booking details. Avoid vague wellness adjectives.

## Section Anatomy

- **Hero:** sand-cream ground, sage eyebrow ("Spa · retreat · stay"), display title, two-line lede, primary CTA ("Book a Stay") + ghost link ("Treatments").
- **Treatments / packages:** card grid with treatment name, duration, brief description, price.
- **Nature / location:** paragraph and image showing the setting — forest, coast, mountain, lake.
- **Wellness program:** retreat formats, group classes, daily schedule snapshot.
- **Gallery:** spa, rooms, pool, landscape, food. Lean into natural light and large breathing room.
- **Booking:** direct booking link, hours, address, phone. Mention cancellation policy.

## Avoid

- Vague wellness language ("rejuvenate", "transformative experience") without concrete details.
- High-saturation tropical imagery (this is sage/teal, not beach club).
- Stock photography of generic massage tables.
- Heavy chrome or shiny luxury detail.
