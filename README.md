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

## Search engine visibility (SEO)
The site is set up to be indexed by Google, Bing, etc. and to surface for queries like
"Blood Flow Imaging", "Blood Flow Imaging Aarhus", "Neurophotonics Aarhus", and "Dmitry Postnov":

- Descriptive `<title>`, meta description and keywords, Open Graph + Twitter cards.
- Structured data (JSON-LD) describing the lab (ResearchOrganization), the PI
  (Person — Dmitry Postnov, with links to LinkedIn / Google Scholar / ResearchGate),
  and the website, so search engines can recognise them as entities.
- `robots.txt` (allows all crawlers) and `sitemap.xml`.
- The canonical URL, `og:url`, `og:image` and JSON-LD URLs are filled in automatically
  with the live address, so they are correct on whatever domain you deploy to — no edit needed.

### One-time steps to get indexed faster
1. **(Optional) Set your real URL** in two files if it differs from the placeholder
   `https://blood-flow-imaging.github.io/`: edit the `Sitemap:` line in `robots.txt`
   and the `<loc>` in `sitemap.xml`.
2. **Google Search Console** (https://search.google.com/search-console): add your site,
   verify ownership (easiest: the "HTML tag" method — paste the provided
   `<meta name="google-site-verification" ...>` tag into the `<head>` of `index.html`),
   then submit `sitemap.xml`.
3. **Bing Webmaster Tools** (https://www.bing.com/webmasters): add the site (you can import
   from Google Search Console) and submit the sitemap.
4. **Get a few inbound links** — e.g. from your Aarhus University staff page, your Google
   Scholar profile, and a LinkedIn post. Inbound links are the strongest signal for fast
   indexing and ranking on name queries.

Indexing typically takes a few days to a couple of weeks after submission.

## Editing
All text lives in `index.html`. Update copy there directly.
