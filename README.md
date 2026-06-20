# Jayesh Koli — Portfolio

Personal static portfolio site built as a single-page HTML/CSS project.

## Contents
- `index.html` — main site
- `assets/` — images and PDFs (including `assets/resume.pdf`)

## Run locally
1. Open `index.html` directly in a browser, or run a local server from the repository root:

```bash
# Python 3
python -m http.server 8000

# then open http://localhost:8000
```

## Update / Deploy
- This repository is designed to be served as a static site (GitHub Pages, Netlify, Vercel, etc.).
- If you update `assets/resume.pdf`, commit and push to `main`. Example:

```bash
git add assets/resume.pdf
git commit -m "Update resume"
git push origin main
```

- If the live site still shows the old file, try:
	- Hard refresh the page (Ctrl+F5) or open in an Incognito window.
	- Purge the CDN cache in your hosting dashboard (Netlify/Cloudflare/Vercel).
	- Force a Pages redeploy by pushing an empty commit:

```bash
git commit --allow-empty -m "trigger redeploy"
git push
```

## Resume troubleshooting
- The resume file is `assets/resume.pdf` and is linked from the nav in `index.html`.
- If you replaced the file but the site didn't update, the cause is usually client or CDN caching — the steps above resolve it.

## Notes
- License: MIT
- Author: Jayesh Koli

## Live Demo

- [Live site](https://jayeshkoli-1402.github.io/portfolio/)


