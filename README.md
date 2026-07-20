# Buyerwise Material Test Standard (MTSR-01) — PWA

This folder is a ready-to-install Progressive Web App.

## Important: this must be hosted over HTTPS
Chrome will **not** offer "Add to Home Screen" (and the service worker
won't register) for a file opened directly from disk (`file://...`).
It needs to be served from a real HTTPS URL. The easiest free option:

### Option A — GitHub Pages (free, ~5 minutes)
1. Create a new GitHub repository (public or private).
2. Upload all 5 files in this folder (`index.html`, `manifest.json`,
   `service-worker.js`, `icon-192.png`, `icon-512.png`) to the repo root.
3. Go to **Settings → Pages**, set Source to the `main` branch, root folder.
4. Wait a minute, then open the URL GitHub gives you
   (e.g. `https://yourname.github.io/your-repo/`).

### Option B — Any static host
Netlify, Vercel, Cloudflare Pages, or your own web/intranet server all
work — just upload these 5 files as-is to the same folder (no build
step needed).

## Installing on Android
1. Open the hosted URL in **Chrome** on the Android device.
2. Tap the **⋮** menu → **"Add to Home screen"** (or Chrome may prompt
   automatically after a moment).
3. Confirm. The app now has its own icon (blue MTSR badge) in the app
   drawer/home screen, opens full-screen with no browser bar, and
   works offline after first load.

Data is stored locally on the device via `localStorage`, same as
before — nothing is sent to a server.
