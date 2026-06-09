# Rustic Farmhouse Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Farm-to-table restaurants, farmhouse inns, rural stays, and countryside venues.

## Visual Direction

Honest, grounded, seasonal, and rural. The page should feel like a converted barn at noon — cream walls, barn-brown beams, terracotta accents, sage-olive trim. Local produce, weather, and season are part of the brand.

## Theme Mode

- **Primary mode:** light
- **Why:** the cream/terracotta/olive palette is daylit by design. The brand is "countryside hospitality", which reads warmer and more grounded on a light ground.
- **How to apply in the consuming project:**
  - Set default `data-mode` to `'light'` in `src/index.html`, persist `'light'` to `localStorage` for `app-mode`.
  - Tune the `:root` block in `src/styles/_theme.scss` to the Palette below.
  - Tune `html[data-mode='dark']` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#F5EDE3` (cream)
- `--c-bg-secondary`: `#FBF6EA`
- `--c-bg-tertiary`: `#EAD8C0`
- `--c-text-strong`: `#6B4423` (barn brown)
- `--c-text`: `#4A2F18`
- `--c-text-muted`: `#8A6E55`
- `--c-primary`: `#B8733C` (terracotta — primary accent)
- `--c-secondary`: `#7A8A5A` (sage olive — secondary accent)
- `--c-border`: `#D9C5A8`
- `--shadow-md`: `0 8px 20px rgba(107, 68, 35, 0.12)`
- `--focus-ring`: `0 0 0 3px rgba(184, 115, 60, 0.45)`

## Secondary Mode Fallback

Dark mode for evening barn dining: `--c-bg-primary` `#2A1E14`, `--c-bg-secondary` `#3A2A1E`, `--c-text-strong` `#F5EDE3`, `--c-text` `#D9C5A8`, `--c-border` `#4A3624`. Keep terracotta and olive accents.

## Typography

- **Display:** `Fraunces`, `Lora`, or a friendly slab. Demo uses `'Segoe UI'`. Weight 600.
- **Body:** `Inter` or `Lora`, weight 400, line-height 1.65.
- **Voice:** honest and concrete. Mention the farm, the season, the producers, the dish, the country roads. Avoid romantic platitudes.

## Section Anatomy

- **Hero:** cream ground, terracotta eyebrow ("Farm to table · since 1991"), display title, two-line lede, primary CTA ("Book a Table") + ghost link ("This Week's Menu").
- **Today's menu / seasonal:** what's on the board this week, with producer credits.
- **The farm / sourcing:** paragraph on the producers, the kitchen garden, what's in season.
- **Stay / inn** (if applicable): rooms, breakfast, walks, returning-guest details.
- **Gallery:** food, kitchen, garden, surrounding countryside.
- **Visit:** address, directions for rural location, hours, phone, reservation method.

## Avoid

- Generic "farmhouse" branding without specific producers or seasonal items.
- High-gloss food styling — this brand is honest, slightly imperfect, real.
- Decorative chalkboard-script fonts or barnyard clip art.
- Hiding the rural location — surface directions and driving guidance.
