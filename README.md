# World's Eye — Global Camera Explorer

A mobile-first Progressive Web App for discovering public webcams around the world. Designed for static hosting on GitHub Pages.

## Features
- Responsive dark dashboard with catalogue statistics
- Worldwide interactive map with indexed camera markers
- Search across camera names, countries and category metadata
- Category shortcuts for city, coastal, wildlife, traffic and mountain cameras
- Country, stream-format and sort filters
- HLS playback where the provider permits embedding, YouTube embeds, and source-page fallback
- Saved cameras stored locally on the device
- Near-me camera sorting (requires location permission and HTTPS)
- External worldwide camera directories for broader coverage
- PWA manifest, service worker and existing app icons

## Deploy to GitHub Pages
1. Extract this ZIP.
2. Upload the **contents** of the `worlds-eye` folder into the root of your GitHub repository (so `index.html`, `cameras.json`, `manifest.json`, `sw.js` and `icons/` are at the repository root).
3. In GitHub, open **Settings → Pages** and select deploy from your main branch and `/ (root)`.
4. Open the published Pages URL in Safari on iPhone, tap **Share → Add to Home Screen**.

## Notes and limitations
- The bundled `cameras.json` catalogue is static and is not a claim that every listed feed is currently live. This app does not automatically add every camera in the world.
- Broad coverage is supplemented with links to external public webcam networks. Provider terms, embedding rules, availability and geographic coverage differ.
- HLS playback uses the hls.js CDN in browsers without native HLS support; iOS Safari can play supported HLS natively. YouTube embeds use YouTube's privacy-enhanced embed host. Some providers block embedded playback; use **Source ↗** or the player fallback.
- The map uses Leaflet and OpenStreetMap tiles. External network access is needed for map tiles and external providers.
- GitHub Pages is static hosting: automated catalogue refresh, scheduled feed health checks, secrets and backend API integrations require a separate backend or permitted public APIs.
- Saved cameras are local to each browser/device and may not sync across devices.
