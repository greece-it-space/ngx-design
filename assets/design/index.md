# Angular Project Design Catalog AI Selector Brief

Use this file when an AI agent needs to choose an Angular project design direction before modifying an Angular 21+ project.

The visual demos live at the same origin as this file. Each design also has a detailed implementation brief under `/assets/design/<slug>.md`.

## How To Choose

1. Identify the real project type, audience, and business model.
2. Identify the expected market position: casual, family, local, premium, luxury, wellness, event-focused, or design-led.
3. Pick one primary design direction from the list below.
4. Open that design's detailed markdown brief.
5. Adapt the target project with its own real content, routes, assets, SEO metadata, contact details, and booking/order links.

Do not merge several directions unless the user explicitly asks for a hybrid. A clear single direction usually produces a better website.

## Global Angular Rules

- Use Angular 21+ standalone components.
- Do not add NgModules.
- Use `ChangeDetectionStrategy.OnPush`.
- Use signals for local UI state.
- Use native control flow: `@if`, `@for`, `@switch`.
- Prefer Tailwind utilities for layout, spacing, typography, sizing, and responsive behavior.
- Keep browser-only code guarded or event-only so prerender remains safe.
- Use `NgOptimizedImage` for static images when feasible.
- Keep pages static, content-first, SEO-friendly, and mobile-readable.

## Design Options

### Cafe Bakery

- Demo route: `/cafe-bakery`
- Brief: `/assets/design/cafe-bakery.md`
- Best for: coffee shops, pastry venues, breakfast cafes, and neighborhood bakeries.
- Choose when the business should feel warm, friendly, bright, handmade, and welcoming.
- Primary theme mode: light.

### Cozy Family

- Demo route: `/cozy-family`
- Brief: `/assets/design/cozy-family.md`
- Best for: family restaurants, small cafes, guest houses, and casual dining places.
- Choose when the site should feel relaxed, practical, comfortable, and trustworthy for everyday visitors.
- Primary theme mode: light.

### Fine Dining

- Demo route: `/fine-dining`
- Brief: `/assets/design/fine-dining.md`
- Best for: chef-led restaurants, tasting menu venues, and premium culinary brands.
- Choose when the business needs refined, quiet, editorial, premium presentation.
- Primary theme mode: light.

### Modern Minimal

- Demo route: `/modern-minimal`
- Brief: `/assets/design/modern-minimal.md`
- Best for: modern restaurants, design hotels, minimalist cafes, and focused hospitality brands.
- Choose when clarity, restraint, whitespace, and direct UX matter more than decorative atmosphere.
- Primary theme mode: light.

### Classic Elegant

- Demo route: `/classic-elegant`
- Brief: `/assets/design/classic-elegant.md`
- Best for: premium traditional restaurants, boutique hotels, and private hospitality events.
- Choose when the business should feel timeless, polished, formal, and reliable.
- Primary theme mode: light.

### Traditional Local

- Demo route: `/traditional-local`
- Brief: `/assets/design/traditional-local.md`
- Best for: national cuisine restaurants, family inns, ethnic cafes, and local hospitality.
- Choose when the business depends on heritage, regional identity, tradition, and authentic local atmosphere.
- Primary theme mode: light.

### Event Banquet

- Demo route: `/event-banquet`
- Brief: `/assets/design/event-banquet.md`
- Best for: wedding venues, banquet halls, conferences, and celebration spaces.
- Choose when the website must sell event formats, capacity, packages, and inquiry flow.
- Primary theme mode: light.

### Boutique Hotel

- Demo route: `/boutique-hotel`
- Brief: `/assets/design/boutique-hotel.md`
- Best for: design hotels, intimate guesthouses, city stays, and personalized hospitality.
- Choose when the business sells rooms, atmosphere, location, amenities, and direct booking.
- Primary theme mode: light.

### Resort Spa

- Demo route: `/resort-spa`
- Brief: `/assets/design/resort-spa.md`
- Best for: wellness hotels, spa sanctuaries, nature retreats, and resort hospitality.
- Choose when the brand should feel calm, natural, restorative, and wellness-focused.
- Primary theme mode: light.

### Rustic Farmhouse

- Demo route: `/rustic-farmhouse`
- Brief: `/assets/design/rustic-farmhouse.md`
- Best for: farm-to-table restaurants, farmhouse inns, rural stays, and countryside venues.
- Choose when local produce, countryside atmosphere, seasonal food, and grounded hospitality are central.
- Primary theme mode: light.

### Luxury Dark

- Demo route: `/luxury-dark`
- Brief: `/assets/design/luxury-dark.md`
- Best for: exclusive restaurants, high-end lounges, private clubs, and luxury venues.
- Choose when the business needs dramatic, dark, exclusive, premium presentation with strong contrast.
- Primary theme mode: dark.

### Speakeasy Cocktail

- Demo route: `/speakeasy-cocktail`
- Brief: `/assets/design/speakeasy-cocktail.md`
- Best for: speakeasies, cocktail bars, hidden bars, and mixology dens.
- Choose when the business should feel candlelit, confidential, and hand-crafted with oxblood and aged-brass atmospherics.
- Primary theme mode: dark.

### Neon Night

- Demo route: `/neon-night`
- Brief: `/assets/design/neon-night.md`
- Best for: late-night izakaya, ramen bars, Asian fusion eateries, and club-adjacent venues.
- Choose when the brand needs electric, neon-sign energy with magenta and cyan accents on jet black.
- Primary theme mode: dark.

### Wine Cellar

- Demo route: `/wine-cellar`
- Brief: `/assets/design/wine-cellar.md`
- Best for: wine bars, enotecas, sommelier-led venues, and tasting rooms.
- Choose when the venue is wine-forward and should feel like a candlelit, scholarly cellar.
- Primary theme mode: dark.

### Smokehouse Ember

- Demo route: `/smokehouse-ember`
- Brief: `/assets/design/smokehouse-ember.md`
- Best for: steakhouses, BBQ joints, grill houses, and smoked-meat venues.
- Choose when the brand is meat-forward and should feel like charcoal, ember, leather, and bronze.
- Primary theme mode: dark.

### Industrial Brewery

- Demo route: `/industrial-brewery`
- Brief: `/assets/design/industrial-brewery.md`
- Best for: craft breweries, taprooms, gastropubs, and beer halls.
- Choose when the venue should feel like a working brewhouse: concrete, iron, copper, no marketing gloss.
- Primary theme mode: dark.

### Jazz Lounge

- Demo route: `/jazz-lounge`
- Brief: `/assets/design/jazz-lounge.md`
- Best for: piano bars, live-music supper clubs, hotel lounges, and listening rooms.
- Choose when the venue is music-led at evening tempo and should feel intimate and smooth.
- Primary theme mode: dark.

### Dark Roast Coffee

- Demo route: `/dark-roast-coffee`
- Brief: `/assets/design/dark-roast-coffee.md`
- Best for: third-wave coffee roasters, evening coffee bars, and dessert cafes.
- Choose when the venue is roast-forward and should feel like an evening roastery rather than a bright cafe.
- Primary theme mode: dark.

### Omakase Black

- Demo route: `/omakase-black`
- Brief: `/assets/design/omakase-black.md`
- Best for: sushi omakase counters, kaiseki rooms, and Japanese fine dining.
- Choose when the venue is chef-led, tasting-format, and should feel precise, quiet, and ceremonial.
- Primary theme mode: dark.

### Botanical Bar

- Demo route: `/botanical-bar`
- Brief: `/assets/design/botanical-bar.md`
- Best for: plant-forward bars, garden restaurants at night, and botanical cocktail rooms.
- Choose when the cocktail program is plant- and herb-led and the room should feel like a night-time greenhouse.
- Primary theme mode: dark.

### Whisky Den

- Demo route: `/whisky-den`
- Brief: `/assets/design/whisky-den.md`
- Best for: whisky bars, cigar lounges, hotel cigar rooms, and members-only nightcap venues.
- Choose when the venue is late-hour and discreet, with quiet authority rather than flashy luxury.
- Primary theme mode: dark.

## Selection Shortcuts

- Bakery, coffee, pastry, brunch: choose `cafe-bakery`.
- Kids, casual family meals, everyday hospitality: choose `cozy-family`.
- Chef, tasting menu, premium cuisine: choose `fine-dining`.
- Contemporary, restrained, design-led: choose `modern-minimal`.
- Formal, traditional premium, timeless service: choose `classic-elegant`.
- National cuisine, heritage, local tradition: choose `traditional-local`.
- Weddings, banquets, conferences, packages: choose `event-banquet`.
- Rooms, guest experience, city stay: choose `boutique-hotel`.
- Spa, wellness, retreat, nature resort: choose `resort-spa`.
- Countryside, farm-to-table, rural inn: choose `rustic-farmhouse`.
- Exclusive lounge, private venue, luxury nightlife: choose `luxury-dark`.
- Prohibition-style, hidden bar, cocktail den: choose `speakeasy-cocktail`.
- Late-night Asian, izakaya, ramen, neon energy: choose `neon-night`.
- Wine bar, enoteca, sommelier-led venue: choose `wine-cellar`.
- Steakhouse, BBQ, grill house, smoked meats: choose `smokehouse-ember`.
- Craft brewery, taproom, gastropub, beer hall: choose `industrial-brewery`.
- Piano bar, supper club, live-music lounge: choose `jazz-lounge`.
- Third-wave roastery, evening coffee bar: choose `dark-roast-coffee`.
- Sushi omakase, kaiseki, Japanese fine dining: choose `omakase-black`.
- Plant-forward bar, garden cocktail room: choose `botanical-bar`.
- Whisky bar, cigar lounge, members nightcap: choose `whisky-den`.

## Theme Mode Guidance For AI Agents

Each detailed brief now declares a primary theme mode (light or dark) and how to tune `src/styles/_theme.scss` and `src/index.html` in the consuming project.

When adopting a design into a real project, the agent must:

1. Read the chosen design's `Theme Mode`, `Palette`, and `Secondary Mode Fallback` sections.
2. Set the project's default `data-mode` on `<html>` (in `index.html`) and `localStorage.app-mode` to the brief's primary mode.
3. Update the primary mode token block in `src/styles/_theme.scss` (`:root` for light, `html[data-mode='dark']` for dark) with the brief's `Palette` values.
4. Update the secondary mode token block with the `Secondary Mode Fallback` values so theme toggling still produces a coherent variant of the same brand.
5. Apply the brief's `Typography` choices via the `--ff-base` token and any per-component overrides.

Do not skip the secondary mode tuning. A consuming project that ships only one mode but leaves the other untouched will look broken if a user toggles the theme.

## Output Expectations For AI Agents

After selecting a design, the agent should:

- state which design it selected and why
- open or use the detailed design brief for that slug
- replace demo content with the target business content
- keep contact, menu, booking, delivery, event, or room information in crawlable text
- preserve Angular 21+ and prerender-safe implementation patterns
- avoid adding CMS, auth, dashboard, API fetching, or heavy state management unless explicitly requested
