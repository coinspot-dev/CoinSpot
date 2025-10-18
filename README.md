# CoinSpot — Believe Ecosystem Tracker

A lightweight, static web app for showcasing trending coins, new launches, and a live trades feed for the **Believe** ecosystem.

## ✨ Features
- Clean Tailwind-based UI, mobile-first
- Trending table with sort (by change / volume)
- New Coins showcase (sample data)
- Live Trades feed (simulated fallback)
- Modal CTA to deep-link to trading
- Works on GitHub Pages / Cloudflare Pages out of the box

## 📁 Project Structure
```
.
├── index.html
└── assets/
    ├── coinspot-icon.png      # App icon / favicon
    └── believe-logo.png       # Round Believe “B” logo
```

## 🚀 Deploy (Cloudflare Pages + GitHub)
1. Push this folder to a GitHub repo (e.g. `CoinSpot`).
2. In Cloudflare Dashboard → **Workers & Pages → Create application → Pages project**.
3. Connect to your GitHub repo, choose the repo.
4. Build settings:
   - **Framework preset:** None
   - **Build command:** (leave empty)
   - **Build output dir:** `/` (root)
5. Deploy. The site will be available at `<project>.pages.dev`.
6. Add a custom domain if needed.

## 🧑‍💻 Local Preview
Just open `index.html` in your browser. No build step required.

## 🔌 Hooking Real Data
- Replace fallback arrays in `index.html` with your real API calls (Believe endpoints).
- Keep the same object keys: `{ name, symbol, price, change, volume, cap }` to avoid breaking the UI.

## 🐛 Common Gotchas
- If buttons don’t respond on mobile webviews: ensure `type="button"` and avoid overlays (z-index issues). Already handled here.
- Favicon not showing? Make sure the PNG exists at `./assets/coinspot-icon.png` and clear browser cache.

## 📄 License
MIT — do whatever you want, attribution appreciated.
