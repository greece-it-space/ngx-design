# Omakase Black Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Sushi omakase counters, kaiseki rooms, Japanese fine dining, and chef-led tasting menu Japanese restaurants.

## Visual Direction

Precise, quiet, ceremonial. The page should feel like a sumi-ink scroll: deep black ground, rice-paper text, a single lacquer-red accent, and bamboo green used sparingly. Every element earns its place; restraint is the design.

## Theme Mode

- **Primary mode:** dark
- **Why:** the sumi-ink/rice-paper contrast is the entire visual identity. Light mode inverts the metaphor (paper → ink) and loses the meditative tone the page is meant to set.
- **How to apply in the consuming project:**
  - Default `data-mode` to `'dark'`, persist `'dark'` in `localStorage` for `app-mode`.
  - Tune `html[data-mode='dark']` in `src/styles/_theme.scss` to the Palette below.
  - Tune `:root` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#101010` (sumi ink)
- `--c-bg-secondary`: `#1A1A1A`
- `--c-bg-tertiary`: `#262626`
- `--c-text-strong`: `#F5F1E8` (rice paper)
- `--c-text`: `#C9C2B0`
- `--c-text-muted`: `#7A7568`
- `--c-primary`: `#8E1F1F` (lacquer red — primary accent)
- `--c-secondary`: `#3A5A3A` (bamboo green — secondary accent)
- `--c-border`: `#262626`
- `--shadow-md`: `0 10px 30px rgba(0, 0, 0, 0.55)`
- `--focus-ring`: `0 0 0 3px rgba(142, 31, 31, 0.40)`

## Secondary Mode Fallback

Light mode inverts to a rice-paper ground: `--c-bg-primary` `#F5F1E8`, `--c-bg-secondary` `#FFFFFF`, `--c-text-strong` `#101010`, `--c-text` `#3A3A3A`, `--c-border` `#D9D4C6`. Keep lacquer red and bamboo green accents identical. Light mode reads as a kaiseki menu printed on washi paper.

## Typography

- **Display:** `Cormorant Garamond` or a refined serif for hero titles; weight 400, generous letter-spacing.
- **Body:** `Inter` or `Sora`, weight 400, line-height 1.75.
- **Accents:** if Japanese characters are used, set in `Noto Serif JP` at a smaller size as eyebrow.
- **Voice:** minimal and precise. Course names, seasonal ingredients, brief origin notes. No marketing claims.

## Section Anatomy

- **Hero:** sumi-ink ground, lacquer-red eyebrow ("Counter omakase"), serif display title (often a single sentence), 2-line lede, primary CTA ("Reserve The Counter") + ghost link ("Tonight's Course").
- **Course / menu preview:** numbered course list (1–10). Each: course number (red), course name (serif), 1–2 line description with key ingredient, optional kanji/kana eyebrow.
- **The counter:** short paragraph on chef, sourcing, seasonality. Specific producer/market mentions add weight.
- **Seasonal kaiseki / kaiseki today:** quiet panel describing the current season's theme.
- **Reserve:** address, seating capacity, sittings, deposit policy if applicable, reservation method.

## Avoid

- Saturated photography or busy backgrounds. Black-and-white or low-saturation images only.
- Multi-column layouts at hero — keep one center column.
- Long marketing paragraphs. Each section under 60 words.
- Decorative pattern fills, cherry blossom clip art, or cliched "asian" motifs.
