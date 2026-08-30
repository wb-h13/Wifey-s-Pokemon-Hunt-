# Wifey's Pokémon Hunt — v6 Full Recount

GitHub Pages-ready PWA.

## Deploy / update
1. Upload **everything in this folder** to the root of the GitHub repo and replace the existing files.
2. Commit the changes.
3. GitHub Pages redeploys automatically from `main` / root.
4. Open/reload the installed app. The v6 service worker replaces the v5 cache.

## v6 catalogue audit
- The English/core hunt is no longer dependent only on the old hand-built list.
- On first load, the app queries TCGdex for every English printing linked to the five target evolution families and expands each physical finish/edition into a separately tickable target.
- This catches reprints and later cards such as **Alakazam ex 215/091 (Paldean Fates)** automatically.
- Detailed variants are used when TCGdex supplies them, including Normal, Holo, Reverse Holo, 1st Edition, Shadowless/subtypes, stamped/promotional finishes, special foils and Jumbo where catalogued.
- TCG Pocket/digital-only cards are excluded.
- The result is cached on the phone. Use **↻ Recount** any time to re-audit the live catalogue.
- Existing owned ticks are migrated by matching card name + set + number + finish. The original curated list remains as a fallback so older/exclusive targets are not silently lost if the API has a coverage gap.

## Existing features retained
- Mew glassmorphism wallpaper/UI.
- Expandable variant checklist per card.
- Automatic on-device progress saving.
- JSON backup / restore.
- Foreign-language catalogue using TCGdex's multilingual API.
