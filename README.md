# QR Word Match (no external libraries)
A single-file web app that scans QR codes using the browser's BarcodeDetector. Camera selector included.

## Deploy to Cloudflare Pages
- Put `index.html` at repo root (or in `public/`), set Output Directory accordingly, leave Build Command blank.

## Deploy to Cloudflare Workers (assets-only)
Create `wrangler.jsonc`:
```jsonc
{
  "name": "qr-word-game",
  "compatibility_date": "2025-09-05",
  "assets": { "directory": "." }
}
```
Then `npx wrangler deploy`.
