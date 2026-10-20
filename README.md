# Descent Live (PWA)

A turn-based hex dungeon crawler. Everything is in `index.html`; no build step.

## Run locally
    cd pwa
    python3 -m http.server 8080
Open http://localhost:8080. Service workers need `localhost` or HTTPS.

## Install
Host this folder on any static HTTPS host (GitHub Pages, Netlify, Cloudflare Pages, Vercel).
- Desktop Chrome/Edge: install icon in the address bar.
- Android: browser menu > Install app.
- iOS Safari: Share > Add to Home Screen.

After the first load the game works offline. Runs save in the browser at the start of every round.

## Files
- index.html — the whole game (canvas renderer, rules engine, AI, UI)
- manifest.webmanifest — app name, colors, icons
- sw.js — offline cache (bump VERSION when you change index.html)
- icon-*.png — app icons
