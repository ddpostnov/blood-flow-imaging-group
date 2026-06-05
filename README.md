# Blood Flow Imaging Group — Lab Website

Single-page static website for the Blood Flow Imaging Group at CFIN, Aarhus University.
Plain HTML/CSS/JS — no build step required.

## Files
- `index.html` — the full one-page site (Who we are · Funding · Research · Infrastructure · Team · Join)
- `styles.css` — styling
- `main.js` — navigation, scroll-spy, scroll reveals, video lazy-play
- `assets/` — images and videos

The top navigation buttons jump to each section, and the active section is
highlighted as you scroll.

## Deploy to GitHub Pages
1. Create a new GitHub repository (e.g. `bfi-group`).
2. Upload everything in this folder to the repository root (keep `assets/` intact).
3. Repo → **Settings → Pages**.
4. **Build and deployment → Source → Deploy from a branch**.
5. Branch `main`, folder `/ (root)`, then **Save**.
6. The site goes live at `https://<username>.github.io/<repo>/`.

> For a user/organisation site, name the repo `<username>.github.io` to serve at the root domain.

## Light / dark theme
The site loads in the **light theme by default**. A toggle in the top-right of the
navigation switches between light and dark, and the choice is remembered between
visits (via `localStorage`). Everything else (layout, content, fonts) is shared
across both themes in `styles.css`.

## Editing
All text lives in `index.html`. Update copy there directly.
