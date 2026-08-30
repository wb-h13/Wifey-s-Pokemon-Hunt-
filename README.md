# Wifey's Pokemon Hunt - v9 cache/deployment fix

- Visible BUILD v9 marker in the header.
- Purges old catalogue caches while preserving every ownership tick.
- Service worker now fetches HTML network-first, so GitHub Pages updates cannot be hidden by an old cached index.html.
- Forces a service-worker update on load and reloads once when the new worker takes control.
- Retains v8 strict family validation, 1,200-variant sanity ceiling, and full collector-number formatting.


## v11
- Keeps Eevee only (no Eeveelutions).
- Raises the validated catalogue safety ceiling for the much larger Eevee catalogue.
- Preserves older good catalogue caches as recovery snapshots.
- Never saves the 518-card fallback as a successful recount.


## Eevee audit guard
Independent English audit: 89 Eevee-family card entries / 157 physical variants (ThePriceDex, 15 Aug 2026). With the previous 805-target baseline, the expected fully represented total is 962. The 1,200 global runaway-query guard is retained, plus a 250-target Eevee-only guard. v11 also preserves older known-good core catalogue caches if a recount fails.
