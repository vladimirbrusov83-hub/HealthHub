# Health & Longevity Knowledge Base

An evidence-based health and longevity resource covering Zone 2 training, VO2 max, strength for aging, protein, nutrition, and key health markers. Built by Coach Vladimir Brusov.

**Live site:** https://health.brusovcoach.org

---

## What It Is

Not a performance guide — a longevity guide. The habits built today determine how well you function in 20–30 years. 12 sections of evidence-based, practical knowledge. No supplements hype, no fads.

---

## Tech Stack

| Layer | Choice |
|-------|--------|
| Structure | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox) |
| Interactivity | Vanilla JS (ES6, no frameworks) |
| Fonts | Barlow Condensed + DM Sans (Google Fonts) |
| Backend | None |
| Dependencies | Zero |
| Build step | None |

Single file — all HTML, CSS, and JavaScript in `index.html` (~1,782 lines).

---

## File Structure

```
HealthHub/
├── index.html    All HTML, CSS, and JS (~1,782 lines)
├── robots.txt    Allows all crawlers, references sitemap
└── sitemap.xml   Single URL, lastmod 2026-03-18, priority 1.0
```

---

## Content Sections (12)

| # | Section | Icon | Category | Read Time |
|---|---------|------|----------|-----------|
| 1 | The Core Philosophy | 🌱 | Foundation | 3 min |
| 2 | Core Physical Components | 🏛️ | Foundation | 4 min |
| 3 | Zone 2 Training | 💚 | Cardio | 6 min |
| 4 | VO2 Max & Longevity | 📈 | Cardio | 5 min |
| 5 | Strength for Longevity | 💪 | Strength | 6 min |
| 6 | How Muscle Actually Works | 🔬 | Strength | 5 min |
| 7 | Aging & Muscle Loss | 🕐 | Strength | 5 min |
| 8 | Protein — The Priority | 🥩 | Nutrition | 6 min |
| 9 | Energy Balance | ⚖️ | Nutrition | 4 min |
| 10 | Supplements — What Works | 💊 | Nutrition | 4 min |
| 11 | Key Health Markers | 🩺 | Longevity | 4 min |
| 12 | Quick Reference Numbers | 🔢 | Reference | 2 min |

---

## Features

### Level Filter
Filter bar with **All / Beginner / Intermediate / Advanced** buttons. Dims non-matching cards to 20% opacity (doesn't hide them — keeps context visible).

Cards use `data-level="beginner|intermediate|advanced"` attribute.

### Search
Full-text search across all sections. Hides entire sections that don't match.

### Scroll Progress Bar
3px green left-edge indicator.

### Active Sidebar Nav
`IntersectionObserver` highlights the current section in sidebar as you scroll.

### Mobile Menu
`toggleMenu()` — single function, bound to hamburger + close button + outside click + nav link click.

---

## Design System

Dark green theme — distinct from the dark navy/red used by Powerlifting and FirstPowerMeet hubs.

| Variable | Value | Use |
|----------|-------|-----|
| `--bg` | `#0a0c0b` | Background (near black) |
| `--accent` | `#2d8c4e` | Green — primary CTAs |
| `--accent2` | `#7ecb95` | Light green — secondary |
| `--beginner` | `#2d8c4e` | Green badge |
| `--intermediate` | `#b8940a` | Gold badge |
| `--advanced` | `#c44a2a` | Orange-red badge |

---

## SEO

- **Canonical:** `https://health.brusovcoach.org`
- **Meta description:** present
- **Open Graph:** og:title / og:description / og:type
- **JSON-LD:** `WebPage` schema (minimal)
- **Sitemap + robots.txt:** present

---

## Deployment

```bash
git add index.html
git commit -m "your message"
git push
```

No build step. No environment variables. Auto-deploys on push.

---

## Part of the BrusovCoach Network

| Site | URL |
|------|-----|
| Main coaching site | https://brusovcoach.org |
| Hypertrophy Hub | https://hypertrophy.brusovcoach.org |
| Powerlifting Hub | https://powerlifting.brusovcoach.org |
| First Meet Guide | https://powermeet.brusovcoach.org |
| Rucking Guide | https://ruck.brusovcoach.org |
