# Classic Elegant Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Premium traditional restaurants, boutique hotels, and private hospitality event venues.

## Visual Direction

Timeless, polished, formal, and reliable. The page should feel like a long-standing hotel dining room — ivory walls, warm-brown wood, antique-gold accents, muted-taupe shadow. Nothing modern shouts here.

## Theme Mode

- **Primary mode:** light
- **Why:** ivory + warm brown + antique gold is a daylit interior palette. The "timeless premium" register reads on light; on dark it tips into nightclub luxury.
- **How to apply in the consuming project:**
  - Set default `data-mode` to `'light'` in `src/index.html`, persist `'light'` to `localStorage` for `app-mode`.
  - Tune the `:root` block in `src/styles/_theme.scss` to the Palette below.
  - Tune `html[data-mode='dark']` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#FBF7EF` (ivory)
- `--c-bg-secondary`: `#FFFFFF`
- `--c-bg-tertiary`: `#F4EDDB`
- `--c-text-strong`: `#5A3C2C` (warm brown)
- `--c-text`: `#3A2A1E`
- `--c-text-muted`: `#75695D` (taupe)
- `--c-primary`: `#5A3C2C` (warm brown — primary accent)
- `--c-secondary`: `#B89652` (antique gold — secondary accent)
- `--c-border`: `#DDD1B5`
- `--shadow-md`: `0 10px 24px rgba(90, 60, 44, 0.10)`
- `--focus-ring`: `0 0 0 3px rgba(184, 150, 82, 0.45)`

## Secondary Mode Fallback

Dark mode for evening events: `--c-bg-primary` `#1F1814`, `--c-bg-secondary` `#2D241C`, `--c-text-strong` `#FBF7EF`, `--c-text` `#DDD1B5`, `--c-border` `#3D2F22`. Keep antique-gold accent strong.

## Typography

- **Display:** `Playfair Display` or `Cormorant Garamond`. Demo uses `Georgia`. Weight 600.
- **Body:** `Lora` or `Crimson Text`, weight 400, line-height 1.7.
- **Voice:** formal but not stiff. Tradition, service, longevity. Mention years established, kitchen tradition, signature dishes.

## Section Anatomy

- **Hero:** ivory ground, antique-gold eyebrow ("Since 1962"), serif display title, two-line lede, primary CTA ("Reserve a Table") + ghost link ("The Menu").
- **Tradition / kitchen:** paragraph on heritage, kitchen lineage, signature plates.
- **Menu preview:** classical structure (entrée / main / dessert), real prices.
- **Private events:** highlight banquets, family celebrations, business dinners.
- **Gallery:** interior detail, table settings, service moments — daylit, never moody.
- **Contact:** hours, dress code if applicable, address, phone, reservation link.

## Avoid

- Modern minimalist tropes (extreme whitespace, micro-typography).
- Casual or playful illustrations.
- Marketing claims about "trends" — this design is anti-trend.
- Cluttered card grids; favor classical column rhythm.
