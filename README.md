# Behind the Show – Lights on Fawn

Static page, no build step. Everything in this folder is the site.

## Preview locally
From the project root: `python serve.py` → http://localhost:8080/behind-the-show/

## Deploy to GitHub Pages
1. Create a public repo, e.g. `lights-on-fawn`.
2. Copy the **contents** of this folder (index.html, styles.css, assets/, .nojekyll) to the repo root and push to `main`.
   ```
   git init && git add . && git commit -m "Behind the Show"
   git branch -M main
   git remote add origin https://github.com/<you>/lights-on-fawn.git
   git push -u origin main
   ```
3. Repo → Settings → Pages → Source: *Deploy from a branch*, Branch: `main` / `(root)`.
4. After a minute it's live at `https://<you>.github.io/lights-on-fawn/`.
5. In PulseMesh, add a Button block → that URL → *Open in new tab*.

## Notes
- `og:image` is relative; once you know the final URL, change it to the absolute
  `https://<you>.github.io/lights-on-fawn/assets/badge-1024.png` so link previews show the badge.
- No scripts, no tracking, no live data from FPP or Home Assistant.
- Edit text directly in index.html; colours live at the top of styles.css.
