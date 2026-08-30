# Wifey's Pokémon Hunt

GitHub Pages-ready PWA.

## Deploy / update
1. Upload **everything in this folder** to the root of the GitHub repo (replace existing files).
2. Commit the changes.
3. GitHub Pages redeploys automatically from `main` / root.
4. On the Pixel, open the site in Chrome. If an older installed version is cached, fully close/reopen it; the v4 service worker removes old app caches automatically.

## What is included
- 517-item core English + foreign-only-exclusive checklist.
- Mew glassmorphism wallpaper/UI.
- Automatic on-device progress saving.
- JSON backup / restore.
- Foreign-language catalogue using TCGdex's public multilingual API.
- Supported language selectors: French, Spanish, Spanish (Mexico), German, Italian, Portuguese, Brazilian Portuguese, Portugal Portuguese, Dutch, Polish, Russian, Japanese, Korean, Traditional Chinese, Simplified Chinese, Indonesian and Thai.
- Foreign data is loaded per-language and cached locally after first load. TCGdex coverage varies by language, so the foreign catalogue reflects cards/variants present in that database rather than claiming perfect completeness for every historic regional printing.

Foreign catalogue requires internet for the first load of each language; already-loaded language data is then saved on the device.

## v5 UI update
- Clean translucent Mew wallpaper (no UI baked into the image).
- Multi-finish printings are grouped into one card row.
- Tap a multi-variant card to expand/collapse its variant checklist.
- Each finish (Holo, Reverse Holo, 1st Edition, etc.) is tracked independently.
- The same expandable behaviour is used in the Foreign catalogue.
