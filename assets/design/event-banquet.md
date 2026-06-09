# Event Banquet Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Wedding venues, banquet halls, conference centers, and celebration spaces.

## Visual Direction

Polished, celebratory, organized, and inquiry-led. The page should sell event formats, capacity, packages, and the inquiry flow — ivory backgrounds, deep navy structure, champagne gold detail, cream linen surfaces.

## Theme Mode

- **Primary mode:** light
- **Why:** ivory + navy + champagne gold is built for daylit weddings and gala brochures. The dark variant works for evening galas but a sales-focused inquiry page is more effective on a bright ground.
- **How to apply in the consuming project:**
  - Set default `data-mode` to `'light'` in `src/index.html`, persist `'light'` to `localStorage` for `app-mode`.
  - Tune the `:root` block in `src/styles/_theme.scss` to the Palette below.
  - Tune `html[data-mode='dark']` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#FEFDFB` (ivory)
- `--c-bg-secondary`: `#FAF5EB` (cream)
- `--c-bg-tertiary`: `#F2E8D0`
- `--c-text-strong`: `#1A2847` (deep navy)
- `--c-text`: `#2A3552`
- `--c-text-muted`: `#6A7088`
- `--c-primary`: `#1A2847` (deep navy — primary accent)
- `--c-secondary`: `#D4AF37` (champagne gold — secondary accent)
- `--c-border`: `#E6D9BD`
- `--shadow-md`: `0 12px 28px rgba(26, 40, 71, 0.10)`
- `--focus-ring`: `0 0 0 3px rgba(212, 175, 55, 0.45)`

## Secondary Mode Fallback

Dark mode for evening events: `--c-bg-primary` `#0E1530`, `--c-bg-secondary` `#1A2240`, `--c-text-strong` `#FEFDFB`, `--c-text` `#E6D9BD`, `--c-border` `#28304D`. Keep champagne-gold accent.

## Typography

- **Display:** `Playfair Display` or `Cormorant Garamond`. Demo uses `Georgia`. Weight 600.
- **Body:** `Lora` or `Crimson Text`, weight 400, line-height 1.7. `Inter` is also acceptable for inquiry forms.
- **Voice:** structured and reassuring. Capacities, formats, package inclusions, lead times. Concrete numbers reduce inquiry friction.

## Section Anatomy

- **Hero:** ivory ground, gold eyebrow ("Weddings · Banquets · Corporate"), serif display title, two-line lede, primary CTA ("Request a Date") + ghost link ("View Packages").
- **Formats / capacity:** card grid showing event types (wedding ceremony, reception, gala, conference) with seated/standing capacity and example packages.
- **Packages:** named tiers with inclusions, sample menu links, indicative pricing.
- **Gallery:** real event photography — multiple formats, not just weddings.
- **Inquiry flow:** clear contact form or email link, response time commitment, lead-time guidance, deposit policy.
- **Visit:** address, hours for viewings, on-site tours, parking info.

## Avoid

- Generic stock wedding photography without venue context.
- Hiding pricing entirely — at least give bands or starting points.
- Hard-sell language; clients are already shopping when they land.
- Mixed-purpose CTAs (book a table + book a wedding) on the same surface.
