# Glacier Utility — CLAUDE.md

## Project Overview
Glacier Utility is a static front-end image processing UI with a dark glassmorphism aesthetic. It consists of two standalone HTML files targeting desktop and mobile viewports.

## File Structure
```
ImageResizely/
├── index.html    # Desktop layout (sticky header, 3-column controls, footer)
├── mobile.html   # Mobile layout (fixed header, bottom nav, vertical card stack)
└── CLAUDE.md
```

## Tech Stack
- **Tailwind CSS** — loaded via CDN (`cdn.tailwindcss.com`) with custom theme config inline
- **Google Fonts** — Inter (UI text), Material Symbols Outlined (icons)
- **No build step** — plain HTML, deployable directly via GitHub Pages

## Design System
- Color palette follows Material Design 3 naming (`primary`, `surface`, `on-surface`, etc.)
- Primary accent: `#7dd3fc` (sky-300)
- Background: `#0a0e1a` (deep navy)
- Glass effects via `.glass-card` / `.glass-panel` custom CSS classes using `backdrop-filter: blur`

## Development Guidelines
- Keep both files self-contained — no shared JS or CSS files
- All Tailwind config lives in the inline `<script id="tailwind-config">` block
- Custom CSS classes (`.glass-card`, `.glass-panel`, `.text-glow`) go in the `<style>` block in `<head>`
- Use Material Symbols icon names (text content inside `<span class="material-symbols-outlined">`)
- Avoid hardcoded hex colors in class attributes — prefer the custom color tokens defined in Tailwind config

## Accessibility Targets
- All interactive controls must have associated `<label>` elements or `aria-label`
- Buttons must have descriptive text or `aria-label`
- Maintain WCAG AA contrast ratios (4.5:1 for normal text, 3:1 for large text)

## Deployment
- GitHub Pages compatible — push to `main`/`master` and enable Pages on the repo root
- No server-side processing; image operations are UI mockups only at this stage
