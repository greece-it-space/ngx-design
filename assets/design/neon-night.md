# Neon Night Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Late-night izakaya, ramen bars, Asian fusion eateries, club-adjacent venues, and Tokyo-night styled food spots.

## Visual Direction

Electric, late-night, neon-sign energy. The page should feel like a wet street outside a 2am ramen shop: jet-black surfaces, magenta and cyan signage glow, condensed display type, and a sense of motion held in stillness.

## Theme Mode

- **Primary mode:** dark
- **Why:** neon only reads as neon against dark. The magenta/cyan accents lose their identity on light surfaces and become flat brand colors.
- **How to apply in the consuming project:**
  - Default `data-mode` to `'dark'` in `src/index.html` and persist `'dark'` in `localStorage` for `app-mode`.
  - Tune `html[data-mode='dark']` in `src/styles/_theme.scss` to the Palette below.
  - Tune `:root` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#0A0A0F` (jet)
- `--c-bg-secondary`: `#14141C`
- `--c-bg-tertiary`: `#1E1E2A`
- `--c-text-strong`: `#F2EFFB`
- `--c-text`: `#C8C5D8`
- `--c-text-muted`: `#7A7898`
- `--c-primary`: `#FF2D92` (hot magenta — primary accent, neon)
- `--c-secondary`: `#36E3FF` (electric cyan — secondary accent, neon)
- `--c-border`: `#2A2A3A`
- `--shadow-md`: `0 0 40px rgba(255, 45, 146, 0.18)` (neon-bloom)
- `--focus-ring`: `0 0 0 3px rgba(54, 227, 255, 0.45)`

## Secondary Mode Fallback

Light mode should feel like a printed flyer of the same brand: `--c-bg-primary` `#F4F2FA`, `--c-bg-secondary` `#FFFFFF`, `--c-text-strong` `#0A0A0F`, `--c-text` `#2A2A3A`, `--c-border` `#D8D6E4`. Keep the same magenta and cyan accents but at slightly higher saturation to compensate for the bright background. Drop the neon-bloom shadow.

## Typography

- **Display:** `Bebas Neue` or `Oswald`, condensed sans. Tracking `+0.06em` for titles, uppercase nav.
- **Body:** `Inter` or `IBM Plex Sans`, weight 400.
- **Accents:** `JetBrains Mono` or any monospace for prices, hours, table numbers.
- **Voice:** punchy, lowercase, short — like a neon-sign caption. "open late." "ramen + highballs." No corporate copy.

## Section Anatomy

- **Hero:** tall, dark, eyebrow uses magenta uppercase ("OPEN UNTIL 3AM"), display title in condensed sans, lede 1–2 short lines. Primary CTA pill in magenta, secondary CTA outlined in cyan. A single neon-glow motif (sign-shaped SVG or text-shadow on a word) can replace any photo.
- **Menu strip:** horizontal scroll of dish cards, mono prices, magenta/cyan dividers between sections.
- **Tonight section:** short list of "what's playing" / "now pouring" / "tonight's special" — treat like a chalkboard panel.
- **Location:** map link, hours (emphasize late close), reservation/walk-in line, phone.
- **Footer:** mono small text, cyan and magenta divider hairlines.

## Avoid

- Warm earth tones, pastels, or "cozy" copy.
- Long-form storytelling — keep all copy in short fragments.
- Soft, blurry, or candle-style imagery; lean into hard light, neon, wet pavement.
- Using both accents in the same component at full opacity (they vibrate); pair one accent with neutral text.
