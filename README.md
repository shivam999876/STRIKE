## STRIKE – Website Creative Design (HTML + CSS only)

### Overview
STRIKE is a bold, motion-forward educational courses website built for the "STRIKE Website Creative Design" hackathon. It uses a mobile-first approach, pure HTML and CSS (no JavaScript), and creative yet accessible animations.

### Files
- `index.html`: Semantic structure of the site (header/nav, hero, courses, tracks, why, pricing, footer).
- `styles.css`: Branding tokens, base styles, responsive layouts, animations, focus states, reduced-motion support.

### Quick start
1. Open `index.html` directly in your browser.
2. Optional: serve locally for best font/caching behavior.
   - Example (PowerShell): `python -m http.server 8080`
   - Then open `http://localhost:8080`.

### Design & branding
- Mobile-first creative layout with fluid typography and modern spacing.
- STRIKE brand colors and gradients:
  - Primary indigo `--strike-primary`
  - Accent cyan `--strike-accent`
  - Accent rose `--strike-accent-2`
- Dark, high-contrast canvas with soft surfaces.

### Key features
- CSS-only responsive navigation (checkbox toggle on mobile; inline on larger screens).
- Hero with animated orbs and perspective grid.
- Featured course cards with subtle conic highlight on hover.
- Tracks section using compact cards and icons.
- Why section with pulsing beam and drifting sparks.
- Simple pricing card with gradient emphasis.
- Accessible focus styles and skip link.

### Customize
Edit CSS tokens in `styles.css` under `:root`:
```css
:root {
  --strike-primary: #6C4CF6;
  --strike-accent: #22d3ee;
  --strike-accent-2: #f43f5e;
  --strike-bg: #0b0b12;
  --strike-text: #f5f7ff;
}
```

### Responsiveness
Mobile-first defaults with two breakpoints:
- `@media (min-width: 640px)`: tablet — grid layouts, inline nav.
- `@media (min-width: 960px)`: desktop — expanded grids, larger headlines.

### Animations & motion
- Floating orbs (`@keyframes float`), pulse beam (`@keyframes pulse`), and sparks (`@keyframes spark`).
- Hover treatments on buttons and cards.
- Respects user settings: `@media (prefers-reduced-motion: reduce)` disables animations and transitions.

### Accessibility
- Semantic landmarks (`header`, `main`, `section`, `footer`).
- Skip link to main content and visible focus rings.
- Color contrast tuned for dark theme; interactive targets sized for touch.

### Notes
- No JavaScript is used. All interactions are CSS-based.
- Google Font: Plus Jakarta Sans is loaded via `<link>` in `index.html`.


