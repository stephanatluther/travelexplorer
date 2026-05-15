---
name: frontend-design-zen
description: "Create production-grade interfaces with Japanese Zen minimalism and soft pinkish color palette"
type: skill
---

# Frontend Design: Japanese Zen + Pinkish Aesthetic

A distinctive, production-grade design system that combines Japanese Zen minimalism with a soft pinkish color palette. This skill guides intentional design thinking before implementation, rejecting generic AI aesthetics in favor of calm, balanced, and memorable interfaces.

## Design Philosophy

### Zen Principles
- **Ma (negative space)**: Purposeful emptiness; let whitespace breathe
- **Wabi-sabi**: Beauty in simplicity, incompleteness, and natural decay
- **Yohaku no bi**: Appreciation for what is left unsaid; leave room for imagination
- **Balance**: Asymmetrical harmony; avoid rigid symmetry
- **Nature-inspired**: Natural materials, organic forms, seasonal references

### Pinkish Color Language
- **Sakura**: #FFB7C5 (cherry blossom pink) — primary accent
- **Blush**: #FFC0CB (soft pink) — secondary tone
- **Rose**: #E8B4C8 (muted mauve-rose) — tertiary element
- **Cream**: #FFF5F7 (off-white with pink undertone) — background/negative space
- **Stone**: #9B8B7E (warm taupe) — text, subtle accents

## Before You Code

### 1. Establish Intent
Ask yourself:
- What emotion should this interface evoke? (calm, peaceful, gentle)
- Who is the user? (what brings them peace?)
- What problem does it solve without noise?
- What single element should they remember?

### 2. Define Your Design Pillars

| Pillar | Zen Guidance | Pinkish Execution |
|--------|--------------|-------------------|
| **Typography** | Minimal, refined serif or sans; generous whitespace between letters | Use warm-neutral fonts (e.g., Noto Serif JP, Inter); prioritize readability over complexity |
| **Color** | Restraint; let one hue carry meaning | Primary: Sakura for CTAs/focus. Backgrounds: Cream. Text: Stone. Accents: Rose/Blush sparingly |
| **Layout** | Asymmetrical grid; generous margins; breathing room | Use 3-4 column grid; minimum 48px padding; never fill all space |
| **Motion** | Slow, deliberate; easing curves that decelerate (ease-out); never frantic | Transitions 300-500ms; fade-ins preferred to slides; subtle spring easing for delightful moments |
| **Texture** | Natural, organic; imperfection valued | Subtle grainy overlays; soft shadows; minimal borders; suggest rather than define |

### 3. Avoid Anti-Patterns
❌ Gradients everywhere (use flat, solid pinkish tones)  
❌ Multiple competing focal points (one hero per screen)  
❌ Harsh shadows or bright whites (use Cream; shadows in warm taupe)  
❌ Rapid animations (speed creates anxiety)  
❌ Heavy serif fonts for body text (choose simplicity)  
❌ Saturated, loud colors (pinks should feel like whispers)  

## Color Palette Reference

```
Sakura Pink       #FFB7C5  (Primary CTA, focus states)
Blush Pink        #FFC0CB  (Secondary accents, hover states)
Rose Mauve        #E8B4C8  (Tertiary; backgrounds for sections)
Cream             #FFF5F7  (Main background, negative space)
Stone Gray        #9B8B7E  (Primary text, icons)
Warm White        #FAFAF8  (Card backgrounds, elevated surfaces)
Shadow Taupe      #D4C4B8  (Subtle borders, dividers)
```

## Implementation Guidelines

### HTML Structure
- Use semantic HTML5 (`<nav>`, `<main>`, `<article>`, `<aside>`)
- Minimal nesting; flat component hierarchy where possible
- Always include `lang` and proper `meta` tags

### CSS Principles
```css
/* Use CSS variables for consistency */
:root {
  --sakura: #FFB7C5;
  --blush: #FFC0CB;
  --rose: #E8B4C8;
  --cream: #FFF5F7;
  --stone: #9B8B7E;
  --spacing-base: 0.5rem;
  --shadow-subtle: 0 1px 3px rgba(0,0,0,0.08);
  --shadow-soft: 0 4px 12px rgba(0,0,0,0.1);
  --transition: 400ms cubic-bezier(0.34, 1.56, 0.64, 1);
}

/* Zen approach: start minimal, add only what's needed */
body {
  background: var(--cream);
  color: var(--stone);
  font-family: 'Noto Serif', serif;
  line-height: 1.6;
  letter-spacing: 0.3px;
}

/* Generous whitespace */
main {
  max-width: 720px;
  margin: 0 auto;
  padding: 3rem 2rem;
}

/* Soft shadows, never harsh */
.card {
  background: var(--warm-white);
  border-radius: 4px;
  box-shadow: var(--shadow-subtle);
  padding: 2rem;
  margin-bottom: 2rem;
}

/* Pinkish accent; restrained */
button, a.cta {
  background: var(--sakura);
  color: white;
  padding: 0.75rem 1.5rem;
  border: none;
  border-radius: 4px;
  transition: all var(--transition);
  font-weight: 500;
}

button:hover {
  background: var(--blush);
  box-shadow: var(--shadow-soft);
}
```

### React/Vue Patterns
- Use functional components with hooks
- Keep state shallow; favor composition over complexity
- Separate styling into CSS Modules or Tailwind with custom config
- Prefer `requestAnimationFrame` for scroll/resize handlers over debounce

### Motion Examples
- **Page load**: Fade-in (opacity 0→1) over 400ms, staggered by 100ms per element
- **Button hover**: Background shift + subtle scale (1→1.02) over 200ms ease-out
- **Scroll reveal**: Fade + 20px upward slide, triggered at 80% viewport entry

## Workflow Checklist

- [ ] Define user context and emotional intent
- [ ] Sketch layout on paper (asymmetrical; note whitespace)
- [ ] Choose 2-3 Zen design pillars to prioritize
- [ ] Select exact hex codes from palette; create CSS variables
- [ ] Build mobile-first; test at 320px, 768px, 1200px
- [ ] Review typography: is it readable? Does it whisper or shout?
- [ ] Audit spacing: does negative space feel intentional?
- [ ] Test animations: do they calm or energize? Remove if unsure.
- [ ] Check contrast (WCAG AA minimum); ensure pinkish tones don't fade text
- [ ] Validate HTML; run Lighthouse; check Core Web Vitals

## Example Structure

```
component/
├── index.jsx
├── style.module.css          # Pinkish + Zen tokens
├── README.md                 # Intent, tone, design rationale
└── __tests__/
    └── Component.test.jsx
```

## Resources

- **Typography**: Google Fonts (Noto Serif JP, Inter, Playfair Display)
- **Motion**: Cubic-bezier.com for easing curves
- **Color reference**: Adobe Color, Chroma.js for accessibility checks
- **Zen inspiration**: Japanese gardens, ink paintings, pottery forms

---

**Remember**: The goal is not decorative complexity, but meaningful simplicity. Every element should justify its presence. Every color should serve a purpose. Whitespace is not empty—it's full of intention.
