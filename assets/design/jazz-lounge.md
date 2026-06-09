# Jazz Lounge Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Piano bars, live-music supper clubs, hotel lounges, listening rooms, and jazz bars with food service.

## Visual Direction

Smooth, intimate, evening tempo. The page should feel like a 10pm set at a hotel lounge: midnight blue room, plum velvet booths, brass lampshades, and vintage cream linen. Music first, food and drink in service of the room.

## Theme Mode

- **Primary mode:** dark
- **Why:** the lounge metaphor is inherently low-light. Brass and cream accents need the deep blue ground to register as candlelit; on white they flatten into generic premium colors.
- **How to apply in the consuming project:**
  - Default `data-mode` to `'dark'`, persist `'dark'` in `localStorage` for `app-mode`.
  - Tune `html[data-mode='dark']` in `src/styles/_theme.scss` to the Palette below.
  - Tune `:root` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#0E1530` (midnight blue)
- `--c-bg-secondary`: `#1A2240`
- `--c-bg-tertiary`: `#252E50`
- `--c-text-strong`: `#F2EAD3` (vintage cream)
- `--c-text`: `#C4B898`
- `--c-text-muted`: `#7E7560`
- `--c-primary`: `#B89968` (warm brass — primary accent)
- `--c-secondary`: `#5A2A4A` (plum — secondary accent)
- `--c-border`: `#28304D`
- `--shadow-md`: `0 10px 30px rgba(0, 0, 0, 0.5)`
- `--focus-ring`: `0 0 0 3px rgba(184, 153, 104, 0.40)`

## Secondary Mode Fallback

Light mode reads as a printed concert program: `--c-bg-primary` `#F4EFE0`, `--c-bg-secondary` `#FFF8E8`, `--c-text-strong` `#0E1530`, `--c-text` `#252E50`, `--c-border` `#D6CCAD`. Keep brass and plum accents; they translate well.

## Typography

- **Display:** `Cormorant Garamond` italic for hero and "Tonight's Set" titles. `Playfair Display` works as alternative.
- **Body:** book-serif at 16px (`Crimson Text` or `Lora`), line-height 1.7.
- **Accents:** small caps for set times and musician names ("MIDNIGHT — TRIO").
- **Voice:** intimate, knowledgeable but unforced. Like a host introducing the next set, not a marketer.

## Section Anatomy

- **Hero:** midnight-blue ground, brass eyebrow ("Live music nightly"), italic serif display title, 2-line lede, primary CTA ("Reserve a Booth") + ghost link ("Tonight's Set").
- **Tonight / This Week:** set list with date, artist, set time. Treat like a concert programme — minimal chrome, brass dividers.
- **The room:** atmospheric paragraph + small horizontal photo strip if available. Lean into low-light imagery.
- **Menu preview:** short list of cocktails and supper-club plates. Treat like a wine list — region, name, brief note.
- **Visit / reserve:** address, hours (evenings, late), reservation method, cover policy if applicable.

## Avoid

- Bright daylight imagery or summer-festival energy.
- Generic stock photos of saxophones or pianos in isolation — prefer wide room shots.
- Long bios for every musician; one or two lines is enough.
- Aggressive marketing copy. The lounge sells itself through tempo, not claims.
