# Saar · Market Desk

Personal Indian market desk as an installable PWA (single-page, works offline).

| File | Purpose |
|---|---|
| `index.html` | Saar app |
| `manifest.webmanifest` | PWA manifest (name, colours, icons) |
| `sw.js` | Service worker — caches the app for offline use |
| `icon.svg`, `icon-192.png`, `icon-512.png` | App icons |
| `journal.html` | Previous Trading Journal app |

## Hosting

Serve the folder over HTTPS (e.g. GitHub Pages: Settings → Pages → Deploy from branch `main`, folder `/`).
The service worker only registers over HTTPS, so opening `index.html` from disk works but won't install offline support.
After changing files, bump the cache name in `sw.js` (`saar-v3` → `saar-v4`) so installed copies update.
