# Portfolio — Idris Tafoukt

Personal one-page portfolio (Front-End Angular Developer → Full-stack Lead).

Art direction: **"developer-editorial"** — deep ink background, Space Grotesk +
JetBrains Mono typography, a single coral accent, subtle scroll reveals and a
progress bar. Designed on [claude.ai/design](https://claude.ai/design), then ported
to a standalone static HTML/CSS/JS page.

## Structure

- `index.html` — the complete, self-contained site (no build step, no dependencies).
  Fonts are loaded from Google Fonts; everything else is inline.

## Local preview

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a repository on GitHub (e.g. `portfolio`).
2. From this folder:

   ```bash
   git remote add origin https://github.com/<your-username>/portfolio.git
   git branch -M main
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main** / **/ (root)** → Save.

4. The site goes live within a few minutes at:
   `https://<your-username>.github.io/portfolio/`

> Tip: for a root URL `https://<your-username>.github.io`, name the repository
> `<your-username>.github.io`.
