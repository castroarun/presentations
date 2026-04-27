# Design References — The Td Mockup Library

A growing index of where each mockup's visual language came from, plus a curated list of sites worth studying for future picks. **The presentation-maker agent reads this file before designing any new deck or mockup.**

---

## Mockups in this folder — origins & inspirations

Each entry lists the source(s) the mockup borrowed from, the specific patterns lifted, and any direct credits.

### `01-brutalist.html` — **LIVE** as the home page

- **Lineage:** Pentagram / Massimo Vignelli / Stefan Sagmeister — classic Swiss-meets-American brutalist editorial design.
- **Patterns borrowed:** asymmetric grid, oversized type with no rounded corners, hard 4px black rules, single electric-red accent (`#ff0033`), monospace metadata captions.
- **Why we picked it:** ages well, type-driven (which suits a *Talks & Decks* identity), feels intentionally crafted rather than templated.

### `02-terminal.html`

- **Lineage:** Unix terminal aesthetic (tmux, htop, neovim splash screens), retro CRT phosphor screens.
- **Patterns borrowed:** ASCII box frames, blinking cursor, scanline overlay (repeating-linear-gradient), monospace-everything, prompt-style header.
- **Reference work:** The `hyper` terminal homepage, anything by [The Coding Train](https://thecodingtrain.com/), classic Linux distro install screens.

### `03-cinema.html`

- **Lineage:** Old movie marquee + Broadway playbills + Bodoni Moda romance.
- **Patterns borrowed:** light-bulb edged frame (`background-image` with radial-gradient dots), velvet-and-gold palette, Italian-typography-school italics on emphasis words, "feature presentation" framing.
- **Reference works:** *Wes Anderson opening titles*, vintage Vogue covers, classic Broadway theatre programmes.

### `04-glitch.html`

- **Lineage:** Cyberpunk / Y2K-revival / glitch-art aesthetic.
- **Patterns borrowed:** chromatic aberration on logo (RGB offset via `::before`/`::after` pseudo-elements), neon pink+cyan palette, clip-path corner cuts, gradient buttons.
- **Reference works:** *Cyberpunk 2077 marketing*, [Linear's launch microsite circa 2020](https://linear.app/), early-2020s redesigns of Discord and Replit.

### `05-newspaper.html`

- **Lineage:** Classic broadsheet journalism — *The New York Times*, *The Times of London*, *Le Monde*.
- **Patterns borrowed:** double-rule dateline, multi-column body, drop caps on first paragraph, italic kicker labels, masthead with italic accent letter.
- **Reference works:** [nytimes.com](https://nytimes.com)'s op-ed pages, [the.ink](https://the.ink) newsletter design, *Bloomberg Businessweek*'s editorial spreads.

### `06-transit.html`

- **Lineage:** Wayfinding / transit map design — Massimo Vignelli's NYC Subway map (1972), Harry Beck's London Underground (1933).
- **Patterns borrowed:** colour-coded "lines" (red, blue, green, yellow), circular station markers with thick coloured borders, Helvetica/Frutiger-style sans-serif, route badge pills.
- **Reference works:** [tfl.gov.uk](https://tfl.gov.uk) (TfL design system), [vignelli.com](https://vignelli.com), Mike Kus's transit-style data visualisations.

### `07-blueprint.html`

- **Lineage:** Architectural / engineering technical drawings.
- **Patterns borrowed:** cyan-on-deep-blue grid background (two layered grids — major + minor), title-block in the corner, dimension callouts row, dashed annotation rules, drawing labels (`DRAWING 01 · DECK`).
- **Reference works:** Le Corbusier's *Modulor* drawings, [archdaily.com](https://archdaily.com) project plans, Apple's old hardware patent drawings.

### `08-polaroid.html`

- **Lineage:** Personal scrapbook + analog photography + handwritten journals.
- **Patterns borrowed:** kraft paper background (multiply-blend SVG noise), polaroid-shaped cards with rotation, washi tape strips (positioned absolute, semi-transparent), Caveat handwritten font, postage-stamp circular marks.
- **Reference works:** [The Sketchnote Handbook](https://sketchnotearmy.com) by Mike Rohde, *Bullet Journal* community designs, handcrafted [are.na](https://are.na) channels.

### `09-saas-iris.html`

- **Lineage:** **[resumefilter.vercel.app](https://resumefilter.vercel.app/)** by **Hakim El Hattab** (creator of [Reveal.js](https://revealjs.com)).
- **Patterns borrowed:** sticky frosted-glass header, orange-gradient logo (`#FFAB72 → #FF8838`) on iris/violet primary (`#5B5BD6`), big bold Inter 800 hero with gradient-clip on emphasis words, floating tilted document cards with subtle shadows, premium SaaS landing-page lede pattern.
- **Why notable:** Hakim is one of the most influential designers in the presentation/web-frontend space — Reveal.js is the most-used HTML presentation framework. His own marketing pages are themselves a study guide.

### `10-score-rings.html`

- **Lineage:** Same source — **[resumefilter.vercel.app](https://resumefilter.vercel.app/)**, but focused on the **candidate-card pattern** (their product UI rather than the marketing hero).
- **Patterns borrowed:** SVG circular progress rings (`stroke-dasharray` with variable arc length), animated number counters, score-coloured stops (green/iris/orange), candidate-row layout with rank ring on the left and tags column on the right, dashboard summary stats in masthead.
- **Why notable:** the score-ring + candidate-row layout is one of the most replicable "scoring/ranking" patterns in modern UI — useful any time decks/items need to feel ranked or graded.

### `11-investor-pitch.html`

- **Lineage:** **[pitch.com](https://pitch.com)** — specifically the [Investor Pitch Deck template](https://pitch.com/templates/Investor-Pitch-Deck-52NJt62Vk3cZ5g7Hgb3XGSPG). Pitch (founded 2018 by ex-Wunderlist team) defined the modern startup-pitch-deck aesthetic.
- **Patterns borrowed:** **multi-section pitch-as-page** (cover → numbers → library → CTA, each labelled `01 / 04`, etc.); **alternating high-contrast slides** (light cover → dark stats → light grid → vibrant CTA); jumbo display type (Inter 900 at 7vw+); **violet-bright accent** (`#7c3aed`) on a deep navy `#0e1230`; **stat-grid pattern** with massive coloured numbers (violet/lime/pink/amber); deck thumbnails with **gradient-mesh backgrounds** (radial-gradient ellipses for "spotlight" effects); pitch-deck slide numbering as a UI pattern.
- **Why notable:** Pitch's design system is the de-facto standard for VC/investor pitches in 2024–26. Borrowing this aesthetic makes a deck instantly read as "fundraise-grade" — useful when the user is presenting to investors, exec leadership, or anyone expecting a polished startup story.
- **Note on faithfulness:** Pitch.com's template gallery is JavaScript-rendered, so this mockup was built from general knowledge of Pitch's design language rather than a direct asset extraction. If the user wants a tighter match to a specific template, they can supply screenshots and the mockup can be refined.

---

## Future inspiration — sites worth studying for new picks

These are sites the agent (or you) should study when reaching for a new aesthetic. Each entry includes **what's notable** and **when to consider it**.

### Presentation frameworks & talk archives

| Site | Why notable | When to consider |
|------|-------------|------------------|
| [revealjs.com](https://revealjs.com) | The reference framework. Hakim's demos are minimalist masters | Any deck that needs reveal-style transitions or flying-fragment animations |
| [hakim.se](https://hakim.se) | Hakim El Hattab's personal site — every detail is intentional | Studying restraint and motion design |
| [slides.com](https://slides.com) | Reveal.js's hosted version — see "Featured" decks | Real-world long-form decks |
| [pitch.com](https://pitch.com) | Modern startup pitch-deck templates — the VC-ready standard. **See `11-investor-pitch.html` for a Td port.** | Corporate/funding-style decks |
| [tldraw.com/p/decks](https://tldraw.com) | Hand-drawn aesthetic done well | Workshop / whiteboard-style talks |

### SaaS / product landing pages (visual systems to borrow)

| Site | Why notable | When to consider |
|------|-------------|------------------|
| [linear.app](https://linear.app) | The current high-water mark for minimalist tech sites — sharp shadows, restrained colour, perfect kerning | Any tech/dev-tools talk |
| [stripe.com](https://stripe.com) | The original "premium fintech" aesthetic — gradient meshes, beautiful typography, layered sections | Finance, fintech, payments talks |
| [vercel.com](https://vercel.com) | Modern monochrome with sharp geometric accents | Frontend/infra/AI-tooling talks |
| [resend.com](https://resend.com) | Soft warm gradients with editorial typography | Developer-tools talks with a friendly tone |
| [supabase.com](https://supabase.com) | Greens-and-blacks with playful illustrations | Open-source / community-driven talks |
| [planetscale.com](https://planetscale.com) | Confident dark theme with electric accents | Database / infra talks |

### Editorial & data-journalism (long-form decks)

| Site | Why notable | When to consider |
|------|-------------|------------------|
| [pudding.cool](https://pudding.cool) | The benchmark for explorable data essays — every piece is a design lesson | Field guides, data-heavy talks |
| [bloomberg.com/graphics](https://www.bloomberg.com/graphics) | Newsroom-grade interactive infographics | Markets, economics, anything with charts |
| [nytimes.com/section/upshot](https://www.nytimes.com/section/upshot) | The Upshot — clarity-first data journalism | Anytime you need credibility through restraint |
| [reuters.com/graphics](https://www.reuters.com/graphics) | Tight, professional, fact-first | News-driven or current-affairs talks |
| [feltron.com](https://feltron.com) | Nicholas Felton's annual reports — legendary data design | Personal-data / quantified-self talks |

### Design-driven personal sites

| Site | Why notable | When to consider |
|------|-------------|------------------|
| [rauno.me](https://rauno.me) | Vercel's design lead — every interaction is over-engineered in the best way | Studying micro-interactions |
| [paco.me](https://paco.me) | Paco Coursey's site — soft minimalism with motion | Personal-talk decks |
| [fjord.dev](https://fjord.dev) | Tonal SaaS aesthetic by Mark Larson | Solo-engineer talks |
| [lee.so](https://lee.so) | Lee Robinson — clean, opinion-driven | Tech opinion talks |

### Brutalist / experimental / outliers

| Site | Why notable | When to consider |
|------|-------------|------------------|
| [are.na](https://are.na) | Curator's haven — minimal, library-like | Any talk that's a curation/anthology |
| [readymag.com/showcase](https://readymag.com/showcase) | Editorial sites pushed to art | When you need to break out of conventions |
| [siteinspire.com](https://siteinspire.com) | Curated gallery — endless scroll-fuel | Browsing for direction |
| [godly.website](https://godly.website) | "Inspirational web design" — heavy on experimental | When restraint isn't called for |

### Slide-deck specific (frameworks & inspirations)

| Site | Why notable | When to consider |
|------|-------------|------------------|
| [maaslalani.com/slides](https://maaslalani.com/slides) | Terminal-based slides (slides.go) — ultimate engineer aesthetic | Pure-text talks |
| [marp.app](https://marp.app) | Markdown-based slides, simple themes | Quick technical talks |
| [bespoke.js.org](https://bespoke.js.org) | Hakim's earlier work — same DNA as Reveal.js | Studying patterns |
| [github.com/owickstrom/the-monospace-web](https://github.com/owickstrom/the-monospace-web) | Monospace design system — borrows from terminals | Engineer talks |

---

## Design patterns worth re-using (cross-mockup)

These are specific techniques that can be borrowed into any mockup, regardless of overall aesthetic.

| Pattern | Source | Re-use it for… |
|---------|--------|----------------|
| **Italic-serif gold-gradient emphasis** | Td decks (signature) | Always — this is Arun's signature flourish |
| **Live IST clock in header** | Td decks | Any deck/page where "this is happening now" matters |
| **Pulsing live dot** | Td decks + Score Rings mockup | Indicating active/in-progress states |
| **Frosted-glass sticky header** | SaaS Iris (← ResumeFilter) | Any site with persistent navigation |
| **Floating tilted document stack** | SaaS Iris (← ResumeFilter) | Any "showcase" hero illustrating cards/items |
| **Conic-gradient progress rings** | Score Rings (← ResumeFilter) | Any "scoring" or "completion" UI |
| **ASCII box corners on cards** | Terminal mockup | Adding texture without changing layout |
| **Light-bulb edged frame** | Cinema mockup | Marquee / showcase moments |
| **Chromatic-aberration logo** | Glitch mockup | Energetic branding moments |
| **Drop cap on first paragraph** | Newspaper mockup | Long-form text introductions |
| **Coloured route lines** | Transit mockup | Showing connections / categories visually |
| **Title block with dimensions** | Blueprint mockup | Any "spec sheet" feel |
| **Washi tape on photo** | Polaroid mockup | Personal / scrapbook moments |
| **Stat band in masthead** | Score Rings (← ResumeFilter) | Summarising library/collection at top |
| **Multi-section page-as-pitch** | Investor Pitch (← Pitch.com) | Long landing pages that read as a pitch deck |
| **Alternating-contrast slides** | Investor Pitch (← Pitch.com) | When you want each section to feel like a new "page" |
| **Jumbo coloured stat numbers** | Investor Pitch (← Pitch.com) | Anywhere stats deserve the loudest voice |
| **Gradient-mesh card thumbnails** | Investor Pitch (← Pitch.com) | Deck/feature thumbnails when you don't have real screenshots |
| **Slide numbering as UI** | Investor Pitch (← Pitch.com) | Anywhere "deck-feel" should bleed into a regular page |

---

## How the agent uses this file

The `presentation-maker` agent is wired to:

1. **Read this file before proposing an aesthetic** for a new deck or mockup.
2. **Cite the source** in the final report ("inspired by *X* — see REFERENCES.md").
3. **Append new entries** when it borrows from a site not yet listed — keeping this library growing organically.
4. **Default to the existing mockups** before inventing new ones, picking the one whose origin best matches the talk's mood.

When the user says *"build me a deck like Stripe's"* or *"the Linear vibe"*, the agent should:
- Cross-reference this file
- Pick the closest existing mockup (or note this as a new entry to add)
- Translate the patterns into the slide context (header, slides, deck.html shell)

---

*Last updated: April 2026. Append new entries chronologically per section.*
