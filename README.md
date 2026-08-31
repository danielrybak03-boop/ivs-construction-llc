# IVS Construction LLC — Website

Single-page static site (`index.html`, no build step needed).

## Deploy to GitHub + Vercel

1. Create a new GitHub repo and push this folder to it:
   ```
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
   git push -u origin main
   ```
2. Go to [vercel.com](https://vercel.com), click **Add New → Project**, and import that GitHub repo.
3. Framework preset: choose **Other** (or leave as detected — it's plain HTML, no build command needed).
4. Click **Deploy**. Vercel will host `index.html` at the root automatically.

That's it — no environment variables or build settings required.

## Notes
- The review section stores submitted reviews (including photos) in the visitor's browser via `localStorage`. Reviews are per-device/browser, not shared across all site visitors. If you want reviews visible to everyone, that requires a backend/database — let me know if you'd like help setting that up.
