# CoinSpot — Public Build (v1)
Date: 2025-10-17

## What’s in this build
- Public SEO (no noindex), canonical tag (update to your domain)
- Status banner + Retry if API fails
- Copy CA safe fallback
- Hero gradient, skeleton loaders, debounce search, NEW badge, trending cards

## Deploy
### Cloudflare Pages
1) New project → **Upload assets** → upload this folder.
2) No build command required.

### GitHub Pages
1) New repo → add `index.html` at root → Settings → Pages → Deploy from `main`/root.

### Netlify
Drag & drop the folder to Netlify dashboard.

## Post-deploy
- Update the `<link rel=\"canonical\">` with your real domain.
- Replace OG image with your brand image.
- If you later need staging, add `<meta name=\"robots\" content=\"noindex\">`.
