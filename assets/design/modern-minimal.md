# Modern Minimal Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Contemporary restaurants, design hotels, minimalist cafes, and focused hospitality brands.

## Visual Direction

Clean, spacious, ordered, and direct. The design should remove visual noise and make the offer feel premium through clarity — pure white surfaces, deep charcoal text, restrained dividers, generous whitespace.

## Theme Mode

- **Primary mode:** light
- **Why:** white-space is the design. The "premium through clarity" promise depends on a bright neutral ground. Dark mode is a coherent alternate but reframes the experience.
- **How to apply in the consuming project:**
  - Set default `data-mode` to `'light'` in `src/index.html`, persist `'light'` to `localStorage` for `app-mode`.
  - Tune the `:root` block in `src/styles/_theme.scss` to the Palette below.
  - Tune `html[data-mode='dark']` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#FFFFFF` (pure white)
- `--c-bg-secondary`: `#F9F9F9` (soft gray)
- `--c-bg-tertiary`: `#F2F2F2`
- `--c-text-strong`: `#1A1A1A` (near-black)
- `--c-text`: `#2E2E2E`
- `--c-text-muted`: `#7A7A7A`
- `--c-primary`: `#1A1A1A` (charcoal — primary accent)
- `--c-secondary`: `#7A7A7A` (mid-gray — secondary accent)
- `--c-border`: `#E8E8E8`
- `--shadow-md`: `0 8px 20px rgba(0, 0, 0, 0.06)`
- `--focus-ring`: `0 0 0 3px rgba(26, 26, 26, 0.30)`

## Secondary Mode Fallback

Dark mode keeps the same restraint inverted: `--c-bg-primary` `#0F0F0F`, `--c-bg-secondary` `#1A1A1A`, `--c-text-strong` `#FFFFFF`, `--c-text` `#E0E0E0`, `--c-border` `#2A2A2A`. Avoid any color tint — keep it neutral.

## Typography

- **Display:** `Inter` or `Söhne` / `Manrope`. Demo uses system sans (`-apple-system`, `BlinkMacSystemFont`, `Segoe UI`). Weight 500–600, tight line-height.
- **Body:** `Inter`, weight 400, line-height 1.55. Generous whitespace around blocks instead of decorative padding.
- **Voice:** short headings, restrained body copy, exact details. No filler.

## Section Anatomy

- **Hero:** white ground, single eyebrow line, single message display title, one primary CTA. No hero photo card unless absolutely necessary.
- **Service / offer cards:** short titles, one-line descriptions, no over-styling.
- **Gallery:** restrained image treatment — large breathing room, minimal captions.
- **About:** focused on design, comfort, clarity. Two paragraphs at most.
- **Booking / contact:** one clear next action. Address, hours, phone — typeset like a quiet contact card.

## Avoid

- Decorative gradients, busy backgrounds, loud illustrations.
- Unnecessary hover effects, animation, or transitions over 200ms.
- Multiple competing CTAs per section.
- Justified text, all-caps body copy, or letterspaced paragraphs.
