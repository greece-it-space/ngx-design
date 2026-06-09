# Speakeasy Cocktail Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Prohibition-style cocktail bars, hidden bars, mixology dens, and hotel cocktail rooms.

## Visual Direction

Confidential, candlelit, and hand-crafted. The page should feel like stepping behind a bookcase: dim, intimate, with aged brass and dark wood doing the work, and the menu treated like a private dossier.

## Theme Mode

- **Primary mode:** dark
- **Why:** the palette is built for low light. Cards, hero, and section surfaces all rely on dark wood and oxblood to register as a cocktail-bar interior; the brass accent only reads warm against deep backgrounds.
- **How to apply in the consuming project:**
  - Set `document.documentElement.setAttribute('data-mode', 'dark')` as the default in `src/index.html` and persist `'dark'` to `localStorage` for `app-mode`.
  - Tune the `html[data-mode='dark']` block in `src/styles/_theme.scss` to the Palette below.
  - Tune the `:root` (light fallback) block to the Secondary Mode Fallback below so the toggle stays coherent.

## Palette (token → hex)

- `--c-bg-primary`: `#1A0F0F` (dark wood / smoke)
- `--c-bg-secondary`: `#2B1A1A`
- `--c-bg-tertiary`: `#3A2424`
- `--c-text-strong`: `#F0E6D2` (parchment)
- `--c-text`: `#C9BBA0`
- `--c-text-muted`: `#847A6B`
- `--c-primary`: `#A07C3B` (aged brass — primary accent)
- `--c-secondary`: `#5A1A1A` (oxblood — secondary accent)
- `--c-border`: `#3D2A2A`
- `--shadow-md`: `0 10px 30px rgba(0, 0, 0, 0.55)`
- `--focus-ring`: `0 0 0 3px rgba(160, 124, 59, 0.40)`

## Secondary Mode Fallback

When light mode is toggled, keep the same accents (`#A07C3B` brass, `#5A1A1A` oxblood) and shift surfaces to parchment: `--c-bg-primary` `#F4ECDC`, `--c-bg-secondary` `#FBF6EA`, `--c-text-strong` `#1A0F0F`, `--c-text` `#3D2A2A`, `--c-border` `#D9C8A8`. The light variant should feel like a daylit cocktail-menu print rather than a bright cafe.

## Typography

- **Display:** `Playfair Display`, serif. Tracking `+0.04em`, weight 600–700. Use for hero title and section H2s.
- **Body:** `Inter`, system sans-serif. Weight 400, line-height 1.6.
- **Voice:** confidential, like a handwritten menu note. Short sentences. Cocktail names in title case, ingredients in lowercase.

## Section Anatomy

- **Hero:** dark backdrop with brass eyebrow ("Established 1929" tone), single-line serif title, lede no longer than two lines, single primary CTA ("Reserve a Table") plus a discreet ghost link ("View The Menu"). No hero photo card; rely on a subtle radial vignette or single illustrated motif (cocktail glass, key, decanter).
- **Signature cocktails:** 3-card grid. Card surface `--c-bg-secondary`, brass hairline border, cocktail name in serif, ingredient list in lowercase body, ABV / price as `--c-text-muted` footnote.
- **The room:** atmospheric paragraph + small horizontal photo strip if available. Treat photography muted, never saturated.
- **Visit / reserve:** address, hours (lean into late-night), reservation method (phone, email, link), dress code line.
- **Footer:** small caps, brass divider line, copyright + "by appointment" note.

## Avoid

- Bright primary colors, neon, or playful illustrations.
- Hero photos with daylight or vibrant food shots.
- Multi-line cocktail descriptions; keep them under 15 words.
- Decorative SVG patterns or busy backgrounds that compete with the candlelight feel.
