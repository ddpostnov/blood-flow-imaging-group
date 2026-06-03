# Blood Flow Imaging Group — website

A single-page website for the Blood Flow Imaging Group (CFIN, Aarhus University),
hosted for free on GitHub Pages.

## Files

- `index.html` — the entire website (text, layout, and styling in one file)
- `assets/` — the photos and figures used on the page

## How to publish (GitHub Pages)

1. Create a free account at https://github.com if you don't have one.
2. Create a new **public** repository. A simple name like `lab-website` is fine.
3. On the repository page, choose **Add file → Upload files**, then drag in
   `index.html` and the whole `assets` folder. Commit the changes.
4. Go to **Settings → Pages**. Under "Build and deployment", set
   **Source = Deploy from a branch**, **Branch = main**, **Folder = / (root)**, and Save.
5. Wait ~1 minute. Your site appears at
   `https://YOUR-USERNAME.github.io/lab-website/`

## How to edit later

Open `index.html` in any text editor. The text content lives near the bottom of
the file (after the `<body>` tag) and reads like plain prose inside tags — change
the words between the tags and re-upload the file. To swap a photo, replace the
matching file in `assets/` (keep the same filename) and re-upload it.

## Using your own domain (optional)

Buy a domain (e.g. from Cloudflare or Porkbun, ~$10–15/year), then add it under
**Settings → Pages → Custom domain** and follow GitHub's DNS instructions.
