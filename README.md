# IVS Construction LLC — Website

A single-page site for IVS Construction LLC (Spartanburg, SC).

## Structure

```
index.html           Main page — HTML, CSS, JS, and the logo (embedded as
                      a base64 image) all in one file, so it can never go
                      missing due to a broken file path.
assets/logo-hd.png   Source copy of the logo, kept for reference/editing —
                      not required for the site to work.
```

## Running locally

No build step needed — it's a static site. Just open `index.html` in a browser,
or serve the folder locally, e.g.:

```
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Deploying with GitHub Pages

1. Push this folder to a GitHub repository.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set the source to **Deploy from a branch**,
   pick the `main` branch and the `/ (root)` folder, then save.
4. GitHub will publish the site at `https://<username>.github.io/<repo-name>/`.

## Editing

- Update contact info, copy, or services directly in `index.html`.
- Swap the logo by replacing `assets/logo-hd.png` (keep the same filename,
  or update the `src="assets/logo-hd.png"` references in `index.html`).
