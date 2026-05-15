---
name: frontend-design
description: Create distinctive, production-grade frontend interfaces with a premium European design sensibility — upmarket, confident, and genuinely standout. Use this skill when the user asks to build web components, pages, artifacts, posters, or applications (examples include websites, landing pages, dashboards, React components, HTML/CSS layouts, or when styling/beautifying any web UI). Generates luxurious, editorial, meticulously crafted code and UI design rooted in European sophistication, avoiding generic AI aesthetics.
license: Complete terms in LICENSE.txt
---

This skill guides creation of distinctive, production-grade frontend interfaces that avoid generic "AI slop" aesthetics. Implement real working code with exceptional attention to aesthetic details and creative choices.

The default aesthetic posture is **premium European sophistication**: the quiet confidence of Swiss typographic tradition, the editorial elegance of a Parisian fashion house, the material precision of Italian/Bauhaus modernism, and the hushed luxury of a high-end maison. The work should feel **upmarket and expensive** — and it should genuinely **stand out**. Premium does not mean timid: it means every bold move is earned, deliberate, and flawlessly executed.

The user provides frontend requirements: a component, page, application, or interface to build. They may include context about the purpose, audience, or technical constraints.

## Design Thinking

Before coding, understand the context and commit to a clear, premium aesthetic direction:
- **Purpose**: What problem does this interface solve? Who uses it? What signals "expensive" to that audience?
- **Tone**: Default to an upmarket European register. Pick a clear lineage and push it to its most refined extreme:
  - *Swiss International* — grid-driven, objective, immaculate typographic hierarchy.
  - *Parisian editorial* — couture, magazine-led, dramatic scale contrast, fashion-house restraint.
  - *Italian / Bauhaus modernist* — geometric, material honesty, decisive colour blocking.
  - *Scandinavian* — calm, functional, airy, exquisitely detailed.
  - *Quiet luxury / haute maison* — subdued palette, generous space, jewellery-grade finish.
- **Constraints**: Technical requirements (framework, performance, accessibility).
- **Differentiation**: What makes this unforgettable? Standout in a premium register comes from *one decisive act of confidence* — an arresting typographic scale, a single saturated accent against bone, an unexpected proportion, a dramatic full-bleed moment — never from visual noise.

**CRITICAL**: Choose a clear conceptual direction and execute it with precision. Luxury comes from intentionality and craft, not intensity. Be bold once, then hold the line — everything else stays disciplined and quiet so the bold move reads.

Then implement working code (HTML/CSS/JS, React, Vue, etc.) that is:
- Production-grade and functional
- Visually refined, expensive-feeling, and memorable
- Cohesive with a clear, confident aesthetic point-of-view
- Meticulously detailed — every margin, weight, kern, and hairline rule considered

## Premium European Guidelines

Focus on:

- **Typography**: Treat type as the primary design element and the main source of luxury. Use distinctive, characterful typefaces with European heritage. Pair a high-contrast editorial display serif (e.g. GT Sesto, Canela, Freight Display, Tiempos Headline, PP Editorial, Spectral, Cormorant) with a precise grotesque for body (e.g. Neue Haas Grotesk, Söhne, Suisse Int'l, ABC Diatype, or a well-set Helvetica Neue). Create *drama through scale contrast* — a very large display setting against small, calm body text reads as couture. Tighten display tracking, set generous body line-height, and use a deliberate modular scale (1.333 or 1.5 for editorial drama). Small-caps, oldstyle figures, ligatures, and hanging punctuation are the fine stitching of premium type.

- **Colour & Theme**: Commit to a restrained, expensive palette. Favour warm off-whites and bone (`#F4F1EA`, `#EDE9E0`, `#FBFAF7`), ink and charcoal near-blacks rather than pure `#000`, and muted stone, taupe, and greige neutrals. Allow exactly **one** confident accent — deep ink blue, oxblood, forest, ochre, terracotta, or a precise metallic-adjacent tone — used sparingly but decisively. A dark "maison" theme (deep ink ground, bone text, one accent) reads instantly upmarket. Avoid saturated candy-bright colour and never use purple gradients on white. Use CSS variables for consistency.

```css
:root {
  /* Light "gallery" register */
  --bone: #F4F1EA;
  --paper: #FBFAF7;
  --ink: #1A1815;
  --stone: #8C857A;
  --hairline: #DAD5C9;
  --accent: #2A3A4A;        /* swap for oxblood / forest / ochre per context */
  /* Type & motion */
  --scale-display: clamp(3rem, 8vw, 7rem);
  --ease: cubic-bezier(0.16, 1, 0.3, 1);
  --shadow-soft: 0 18px 48px -24px rgba(26, 24, 21, 0.30);
}
```

- **Motion**: Motion should be discreet and well-mannered — the choreography of a luxury boutique, not an arcade. Prefer slow, eased transitions (300–700ms, custom cubic-bezier easing), subtle fades, and small translations. One quietly orchestrated page-load reveal with staggered timing (mask-reveal of headlines, lines rising into place) outperforms scattered micro-interactions and is the single most effective "premium" cue. Hover states stay understated — a fine underline that draws in, a measured colour shift, a slow image scale. CSS-only for HTML; Motion library for React when available.

- **Spatial Composition**: Lean on the grid, then break it once with intent. Swiss-style columnar layouts, strong baseline alignment, and asymmetric balance read as sophisticated. Use generous — even extravagant — negative space; on a premium site, empty space *is* the luxury. Thin hairline rules (1px), wide editorial margins, index numbers, and considered captions structure the page. A single dramatic full-bleed or oversized element provides the standout moment.

- **Backgrounds & Visual Details**: Create atmosphere through subtlety: warm paper-like background tints, the faintest grain or noise overlay, hairline dividers, restrained soft shadows (low-opacity, never heavy). Fine borders, letter-spaced small-caps labels, index numbers (01 / 02 / 03), and editorial metadata add the craft that signals expense. Avoid glossy effects, neon glows, drop shadows that look cheap, and heavy gradient meshes.

NEVER use generic AI-generated aesthetics like overused font families (Inter as a display face, Roboto, Arial, system fonts), cliched colour schemes (particularly purple gradients on white backgrounds), predictable layouts and component patterns, and cookie-cutter design that lacks context-specific character.

Interpret with taste and make confident, intentional choices that feel genuinely designed for the context. No design should be the same. Vary within the European register — light bone-paper "gallery" themes and deep ink "maison" dark themes, different serif/grotesque pairings, different national sensibilities (Swiss, Nordic, French, Italian). NEVER converge on common choices (Space Grotesk, for example) across generations.

## Anti-Patterns to Avoid

- Purple/blue gradients on white — the surest tell of generic AI design.
- Inter, Roboto, Arial, or system fonts as a display face.
- Symmetrical, centred, single-column "template" layouts with no grid tension.
- More than one accent colour, or accents used everywhere instead of decisively.
- Heavy, dark, blurry drop shadows — they read as cheap.
- Busy surfaces — on premium work, restraint and space are the value.
- Bouncy, fast, or scattered micro-animations — luxury moves slowly.

**IMPORTANT**: Match implementation complexity to the aesthetic vision. A premium European design demands restraint, precision, and careful attention to spacing, typographic scale, and subtle detail — not elaborate effects. Elegance comes from executing a disciplined, confident vision flawlessly.

Remember: Claude is capable of extraordinary creative work. Show what can truly be created when committing fully to a distinctive, upmarket vision — confident, considered, expensive, and quietly unforgettable.
