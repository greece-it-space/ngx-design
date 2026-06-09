# Fine Dining Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Chef-led restaurants, tasting menu venues, premium dining rooms, and exclusive culinary experiences.

## Visual Direction

Refined, editorial, precise, quiet, and premium. The page should create confidence through restraint, strong hierarchy, and carefully selected imagery — champagne ivory walls, deep navy accents, burnished gold detail.

## Theme Mode

- **Primary mode:** light
- **Why:** the palette is ivory-dominant. Navy and gold work as editorial accents on a champagne-ivory ground; light is the brand's resting state. Dark mode is a viable evening variant but should not be the default.
- **How to apply in the consuming project:**
  - Set default `data-mode` to `'light'` in `src/index.html`, persist `'light'` to `localStorage` for `app-mode`.
  - Tune the `:root` block in `src/styles/_theme.scss` to the Palette below.
  - Tune `html[data-mode='dark']` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#FAF8F3` (champagne ivory)
- `--c-bg-secondary`: `#FFFFFF`
- `--c-bg-tertiary`: `#F2EEE3`
- `--c-text-strong`: `#1A1A2E` (deep navy)
- `--c-text`: `#2A2A2A` (charcoal)
- `--c-text-muted`: `#6E6E72`
- `--c-primary`: `#1A1A2E` (deep navy — primary accent)
- `--c-secondary`: `#C9A961` (burnished gold — secondary accent)
- `--c-border`: `#E2DCCB`
- `--shadow-md`: `0 10px 30px rgba(26, 26, 46, 0.10)`
- `--focus-ring`: `0 0 0 3px rgba(201, 169, 97, 0.45)`

## Secondary Mode Fallback

Dark mode for evening service: `--c-bg-primary` `#1A1A2E`, `--c-bg-secondary` `#22223A`, `--c-text-strong` `#FAF8F3`, `--c-text` `#D6D1C3`, `--c-border` `#2D2D45`. Keep gold accent. The dark variant should feel like the same dining room after sundown.

## Typography

- **Display:** `Playfair Display` or `Cormorant Garamond`. Demo uses `Georgia`. Weight 500–600 for editorial restraint.
- **Body:** `Lora` or `Crimson Text` (serif book). Weight 400, line-height 1.7.
- **Voice:** concise and specific. Cuisine direction, chef name, tasting format, pricing band, reservation method. No marketing claims.

## Section Anatomy

- **Hero:** ivory ground, gold eyebrow ("Tasting menu, evenings only"), serif display title, two-line lede, primary CTA ("Reserve A Table") + ghost link ("The Menu").
- **Chef / concept:** short editorial paragraph. Photo treatment low-saturation, never glossy.
- **Tasting menu / signature dishes:** numbered or named courses with brief tasting notes.
- **Wine, pairing, or private dining:** subdued highlight if relevant.
- **Gallery:** food, interior, service. Editorial pacing — fewer images, more space.
- **Reservation / contact:** hours, dress code, address, phone, reservation link.

## Avoid

- Playful decorative UI, overloaded cards, loud colors, or casual copy.
- Stock food photography or overly saturated dish shots.
- "Award-winning", "renowned", "best" — let the chef and menu speak.
- Family-friendly framing.
