# Masoom Sharma — Portfolio

A single-file personal portfolio site for **Masoom Nayanranjan Sharma**, Senior AI/ML &amp; Cloud (AWS) Engineer. Built as one self-contained HTML file — no build step, no dependencies, no framework. Open it in a browser and it runs.

Styled as an engineer's **"control plane"**: a deep ink base, a single restrained signal-amber accent, and a career-pipeline spine, with a subtle attention-matrix shimmer in the hero.

---

## Features

- **Zero dependencies** — one HTML file with inline CSS and vanilla JS. Nothing to install.
- **Fully responsive** — adapts from desktop down to mobile.
- **Accessible** — semantic markup, visible keyboard focus, and `prefers-reduced-motion` support (animation falls back to a single static frame).
- **Animated hero** — a lightweight `<canvas>` attention-matrix that shimmers diagonally; capped at 2× DPR and paused for reduced-motion users.
- **Scroll reveals** — `IntersectionObserver`-driven fade-ins (no scroll-jank libraries).
- **Auto-hiding nav** — hides on scroll-down, reappears on scroll-up.

## Sections

1. Hero — name, role, and thesis
2. Metrics strip — 11+ yrs · 3 AWS credentials · 5 engineers led · BFSI
3. Profile / About
4. Technical stack — grouped by AI/ML, AWS AI &amp; Data, Cloud &amp; Infra, and Data/DevOps
5. Career pipeline — Appsguru → DXC → Accenture
6. Selected work — Loan Default Prediction System
7. Certifications &amp; Education
8. Contact

## Tech

| Layer | Choice |
|-------|--------|
| Markup / styling | Hand-written HTML + CSS (CSS custom properties for theming) |
| Scripting | Vanilla JS (`IntersectionObserver`, Canvas 2D) |
| Display type | [Clash Display](https://www.fontshare.com/fonts/clash-display) (Fontshare) |
| Body type | [Satoshi](https://www.fontshare.com/fonts/satoshi) (Fontshare) |
| Mono / labels | [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) (Google Fonts) |

Fonts load from CDNs at runtime, so an internet connection is needed for the intended typography (the page still renders with system-font fallbacks offline).

---

## Getting started

Clone or download, then open the file — that's it.

```bash
# option 1: just open it
open masoom-sharma-portfolio.html      # macOS
# xdg-open masoom-sharma-portfolio.html # Linux
# start masoom-sharma-portfolio.html    # Windows

# option 2: serve locally (recommended for accurate font/CDN behaviour)
python3 -m http.server 8000
# then visit http://localhost:8000/masoom-sharma-portfolio.html
```

## Before you publish — fill in 3 placeholders

Open `masoom-sharma-portfolio.html` and replace these in the **Contact** section:

| Placeholder | Replace with |
|-------------|--------------|
| `your.email@example.com` | Your real email |
| `https://linkedin.com/in/your-handle` | Your LinkedIn URL |
| `https://github.com/your-handle` | Your GitHub URL |

The phone number and all other content are already filled in.

> Tip: if you rename the file to `index.html`, hosts will serve it automatically at the root URL.

## Deploy

**GitHub Pages**
1. Push the file to a repo (rename to `index.html`).
2. Settings → Pages → deploy from the `main` branch, root folder.
3. Your site goes live at `https://<username>.github.io/<repo>/`.

**Netlify / Vercel** — drag the folder into the dashboard, or connect the repo. No build command; the publish directory is the folder containing the file.

## Customizing

- **Colors** — edit the CSS variables at the top of the `<style>` block (`--ink`, `--signal`, `--text`, etc.). Change `--signal` to re-theme the whole accent.
- **Content** — everything is plain HTML; edit the text directly in each `<section>`.
- **Hero animation** — tune `TARGET` (cell size) and the alpha values inside the matrix `draw()` function near the bottom of the file.

## Accessibility

- Respects `prefers-reduced-motion` (static hero, no reveal transitions).
- Focus-visible outlines on all interactive elements.
- Sufficient contrast between text and the ink background.

---

## Credits

Design &amp; build tailored to Masoom Sharma's résumé. Typefaces by Fontshare (Clash Display, Satoshi) and Google Fonts (JetBrains Mono), used under their respective licenses.
