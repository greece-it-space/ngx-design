# Boutique Hotel Design Brief

> See `index.md` for shared Angular, prerender, and SEO rules. This file is the visual and theme contract for the design.

## Best For

Design hotels, intimate guesthouses, city stays, and personalized hospitality brands.

## Visual Direction

Atmospheric, curated, and personal. The page should sell rooms, atmosphere, location, amenities, and direct booking — ivory and warm-charcoal interior palette, muted-rose accent, soft warm-gray detail. Quiet design, not corporate hotel chain.

## Theme Mode

- **Primary mode:** light
- **Why:** ivory and warm charcoal is a daylit guest-experience palette. The brand promise is "personalized stays" which reads warmer on light surfaces.
- **How to apply in the consuming project:**
  - Set default `data-mode` to `'light'` in `src/index.html`, persist `'light'` to `localStorage` for `app-mode`.
  - Tune the `:root` block in `src/styles/_theme.scss` to the Palette below.
  - Tune `html[data-mode='dark']` to the Secondary Mode Fallback below.

## Palette (token → hex)

- `--c-bg-primary`: `#FAF9F7` (ivory)
- `--c-bg-secondary`: `#FFFFFF`
- `--c-bg-tertiary`: `#F2EFEA`
- `--c-text-strong`: `#3D3D3D` (warm charcoal)
- `--c-text`: `#555555`
- `--c-text-muted`: `#8A8A84` (warm gray)
- `--c-primary`: `#3D3D3D` (warm charcoal — primary accent)
- `--c-secondary`: `#C4B5AC` (muted rose — secondary accent)
- `--c-border`: `#E4DED5`
- `--shadow-md`: `0 12px 28px rgba(61, 61, 61, 0.10)`
- `--focus-ring`: `0 0 0 3px rgba(196, 181, 172, 0.45)`

## Secondary Mode Fallback

Dark mode for evening browsing: `--c-bg-primary` `#1A1A1A`, `--c-bg-secondary` `#262626`, `--c-text-strong` `#FAF9F7`, `--c-text` `#D6D1CA`, `--c-border` `#333030`. Keep muted-rose accent.

## Typography

- **Display:** `Inter` (display weight) or `Söhne`. Demo uses `'Segoe UI'`. Weight 500–600.
- **Body:** `Inter`, weight 400, line-height 1.65.
- **Voice:** atmospheric and specific. Room count, neighbourhood, view, breakfast, amenities, host. No corporate hotel-chain language.

## Section Anatomy

- **Hero:** ivory ground, rose eyebrow ("Eight rooms in the old quarter"), display title, two-line lede, primary CTA ("Book Direct") + ghost link ("View Rooms").
- **Rooms / suites:** small card grid (or list) — name, key features, capacity, starting rate.
- **Neighbourhood:** paragraph on location, walking distance to landmarks, neighbourhood character.
- **Amenities:** breakfast, lounge, wellness, services. Mention what's included vs paid.
- **Gallery:** rooms, communal spaces, neighbourhood, breakfast. Editorial pacing.
- **Direct booking:** booking widget or link, cancellation policy, contact for special requests.

## Avoid

- Big-chain stock photography of generic rooms.
- Hidden cancellation terms — surface the policy in the booking section.
- Loyalty-program prompts before the guest even sees rooms.
- "Luxury" framing if the venue is actually boutique/personal — different register.
