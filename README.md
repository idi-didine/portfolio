# Portfolio — Idris Tafoukt

Portfolio personnel one-page (Développeur Front-End Angular → Lead full-stack).

Direction artistique **« developer-editorial »** : fond encre profond, typographies
Space Grotesk + JetBrains Mono, accent corail unique, révélations subtiles au scroll
et barre de progression. Conçu sur [claude.ai/design](https://claude.ai/design) puis
porté en HTML/CSS/JS statique autonome.

## Structure

- `index.html` — site complet, autonome (pas de build, pas de dépendances).
  Les polices sont chargées depuis Google Fonts ; tout le reste est inline.

## Aperçu en local

Ouvrir `index.html` dans un navigateur, ou servir le dossier :

```bash
python3 -m http.server 8000
# puis ouvrir http://localhost:8000
```

## Publication sur GitHub Pages

1. Créer un dépôt sur GitHub (ex. `portfolio`).
2. Depuis ce dossier :

   ```bash
   git remote add origin https://github.com/<votre-utilisateur>/portfolio.git
   git branch -M main
   git push -u origin main
   ```

3. Sur GitHub : **Settings → Pages → Build and deployment**
   - Source : **Deploy from a branch**
   - Branch : **main** / **/ (root)** → Save.

4. Le site sera en ligne sous quelques minutes à l'adresse :
   `https://<votre-utilisateur>.github.io/portfolio/`

> Astuce : pour une URL racine `https://<votre-utilisateur>.github.io`,
> nommez le dépôt `<votre-utilisateur>.github.io`.
