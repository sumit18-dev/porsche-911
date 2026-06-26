# Porsche 911 — Landing Page (Concept)

A single-file, dark-themed, animated landing page concept for the Porsche 911 lineup. Built with plain HTML, CSS, and vanilla JavaScript — no frameworks, no build step.

> ⚠️ **Disclaimer:** This is an unofficial fan/demo project for design & development practice. It is not affiliated with, endorsed by, or sponsored by Porsche AG. All trademarks, model names, and the Porsche crest/branding belong to their respective owners.

## ✨ Features

- **Responsive hero section** with an animated SVG car, live stat counters, and CTA buttons
- **Model showcase grid** for 6 trims (Carrera, Targa 4, Turbo S, GT3, Cabriolet, GT3 RS) with hover-reveal spec overlays
- **Live-style performance dashboard** with animated counters and progress bars
- **Animated horsepower bar chart** comparing all trims
- **Full specs comparison table** (price, engine, 0–100, top speed, drivetrain, etc.)
- **Heritage timeline** scrolling through the 911's history (1963–2025)
- **Fully responsive** — tablet and mobile breakpoints with a collapsible nav menu
- Smooth scroll, `IntersectionObserver`-driven entrance animations, and no external JS dependencies

## 🛠️ Tech Stack

- **HTML5** — single-file structure
- **CSS3** — custom properties, Grid/Flexbox, keyframe animations, clamp()-based responsive typography
- **Vanilla JavaScript** — counters, chart rendering, nav toggle, scroll-triggered animations
- **Google Fonts** — [Inter](https://fonts.google.com/specimen/Inter)
- **Tabler Icons** — via CDN (`@tabler/icons-webfont`)

No build tools, no package manager, no dependencies to install.

## 📁 Project Structure

```
.
└── porsche-911-landing.html   # everything — markup, styles, and scripts in one file
```

## 🚀 Getting Started

No installation required.

```bash
# Clone the repo
git clone https://github.com/your-username/porsche-911-landing.git
cd porsche-911-landing

# Open directly in your browser
open porsche-911-landing.html      # macOS
start porsche-911-landing.html     # Windows
xdg-open porsche-911-landing.html  # Linux
```

Or just double-click the file. Since it loads fonts/icons from a CDN, an internet connection is needed for full styling.

### Optional: serve locally

```bash
python3 -m http.server 8000
# then visit http://localhost:8000/porsche-911-landing.html
```

## 🎨 Customization

| What | Where |
|---|---|
| Colors / theme | CSS custom properties in `:root` (`--gold`, `--red`, `--dark`, etc.) |
| Model data & specs | Edit each `.model-card` block and the `.compare-table` rows |
| Horsepower chart values | `models` array inside `buildPowerChart()` in the `<script>` |
| Live metric values | `animateCounter()` calls inside the `IntersectionObserver` callback |
| Timeline entries | `.tl-item` blocks inside the `.tl-strip` |

## 📱 Browser Support

Tested on the latest Chrome, Firefox, Safari, and Edge. Uses modern CSS (`clamp()`, `backdrop-filter`, CSS Grid) — not optimized for IE11 or legacy browsers.

## 📄 License

MIT — feel free to fork, modify, and use this as a starting point for your own projects.

## 🙏 Credits

- Desinged By: [Sumit Anand](https://github.com/Sumitanand909) 
- Icons: [Tabler Icons](https://tabler.io/icons)
- Font: [Inter](https://fonts.google.com/specimen/Inter) by Rasmus Andersson
