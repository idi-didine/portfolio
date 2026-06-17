# Portfolio — Idris Tafoukt

Personal one-page portfolio (Front-End Angular Developer → Full-stack Lead).

🔗 **Live:** https://idi-didine.github.io/portfolio/

Art direction: **"developer-editorial"** — deep ink background, Space Grotesk +
JetBrains Mono typography, a single coral accent, subtle scroll reveals and a
progress bar. Designed on [claude.ai/design](https://claude.ai/design), then ported
to a standalone static HTML/CSS/JS page.

## Features

- **One-page layout** — hero, profile, skills, experience timeline, personal
  project, education / languages / interests, and contact.
- **Bilingual (FR / EN)** — a language switcher in the nav toggles all content via
  a client-side dictionary. The first language is auto-detected from the browser
  (English browsers → EN, otherwise French) and the choice is remembered in
  `localStorage`. `<html lang>` and the SEO meta tags update on switch.
- **Subtle motion** — scroll progress bar and on-scroll reveal, both disabled when
  the visitor prefers reduced motion (`prefers-reduced-motion`).
- **Responsive** — adapts the nav and grids down to mobile.
- **SEO / sharing** — descriptive `<title>`, meta description, Open Graph tags and
  an inline SVG favicon.
- **Zero dependencies / no build** — a single `index.html`; only the web fonts are
  fetched from Google Fonts.

## Tech stack

Plain **HTML + CSS + vanilla JavaScript** (no framework, no bundler).
Fonts: Space Grotesk, Hanken Grotesk, JetBrains Mono (Google Fonts).

## Structure

```
.
├── index.html   # the complete, self-contained site (markup, styles, i18n, scripts)
└── README.md
```

## Local preview

Open `index.html` directly in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Customizing the content

- **Text & sections** — edit the markup directly in `index.html`.
- **Translations** — each translatable element carries a `data-i18n="key"`
  attribute; the matching French and English strings live in the
  `I18N = { fr: {...}, en: {...} }` object in the inline `<script>`. Edit both
  languages for a key to change its text.
- **Colors / fonts** — the palette (ink `#0B0B0F`, coral `#FF6A3D`, …) is applied
  inline; the accent color and fonts are easy to find-and-replace.

## Deploy to GitHub Pages

1. Create a public repository named `portfolio` on GitHub.
2. From this folder:

   ```bash
   git remote add origin https://github.com/idi-didine/portfolio.git
   git branch -M main
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main** / **/ (root)** → Save.

4. The site goes live within a few minutes at:
   https://idi-didine.github.io/portfolio/

> Tip: for a root URL `https://idi-didine.github.io`, name the repository
> `idi-didine.github.io` instead.

## Author

**Idris Tafoukt** — Front-End Angular Developer, Bejaïa, Algeria.

- Email: tafouktidris@gmail.com
- LinkedIn: [in/idris-tafoukt](https://linkedin.com/in/idris-tafoukt)

## License

Personal portfolio. The source code may be used as a reference, but the written
content, résumé details and personal branding are © 2026 Idris Tafoukt — please
don't reuse them as your own.
