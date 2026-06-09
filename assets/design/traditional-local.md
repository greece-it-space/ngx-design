# Traditional Local Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

National cuisine restaurants, family inns, ethnic cafes, regional taverns, and local hospitality with heritage character.

## Visual Direction

Heritage, regional, authentic, and grounded. The page should feel like a long-standing country tavern — wheat-cream walls, burgundy red highlights, forest-green tradition, antique gold trim. Pride of place is the design language.

## Theme Mode

- **Primary mode:** light
- **Why:** the wheat/burgundy/forest palette is built around a daytime tavern interior. On dark it tips into theatrical "heritage restaurant" branding that loses the lived-in feel.
- **How to apply in the consuming project:**
  - Set default `data-mode` to `'light'` in `src/index.html`, persist `'light'` to `localStorage` for `app-mode`.
  - Tune the `:root` block in `src/styles/_theme.scss` to the Palette below.
  - Tune `html[data-mode='dark']` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#F4E8C8` (wheat cream)
- `--c-bg-secondary`: `#FBF4DD`
- `--c-bg-tertiary`: `#EAD3AA`
- `--c-text-strong`: `#3A2A1E`
- `--c-text`: `#5A4030`
- `--c-text-muted`: `#806648`
- `--c-primary`: `#8E281F` (burgundy red — primary accent)
- `--c-secondary`: `#2F5B3D` (forest green — secondary accent)
- `--c-border`: `#D9C09A`
- `--shadow-md`: `0 8px 20px rgba(90, 64, 48, 0.12)`
- `--focus-ring`: `0 0 0 3px rgba(178, 123, 44, 0.45)`

## Secondary Mode Fallback

Dark mode for evening trade: `--c-bg-primary` `#2A1E14`, `--c-bg-secondary` `#3A2A1E`, `--c-text-strong` `#F4E8C8`, `--c-text` `#D9C09A`, `--c-border` `#4A3624`. Keep burgundy and forest-green accents.

## Typography

- **Display:** `Lora`, `Playfair Display`, or a regional/national display font if appropriate. Demo uses `Georgia`. Weight 600.
- **Body:** `Lora` or `Crimson Text`, weight 400, line-height 1.7.
- **Voice:** rooted, warm, regional. Mention recipes inherited, ingredients sourced locally, family ownership, holiday menus.

## Section Anatomy

- **Hero:** wheat ground, burgundy eyebrow ("Family tavern since 1958"), serif display title, two-line lede, primary CTA ("Reserve a Table") + ghost link ("Our Recipes").
- **Heritage / kitchen:** paragraph on family, recipes, origin region. Concrete sourcing details where possible.
- **Menu preview:** traditional dishes grouped by course or region, with brief context lines.
- **Local sourcing:** producers, farms, or markets credited by name.
- **Gallery:** interior detail, table settings, traditional dishes, regional landscape.
- **Contact:** address, hours, phone, reservation, holiday hours.

## Avoid

- Pan-cultural "ethnic" decoration that flattens regional identity.
- Modernist tropes — this design is intentionally non-trendy.
- Stock photography of generic "old-world" interiors.
- Family-friendly framing if the venue is wine/spirit-led; calibrate to the real business.
