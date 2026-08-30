# Wifey's Pokemon Hunt - v9 cache/deployment fix

- Visible BUILD v9 marker in the header.
- Purges old catalogue caches while preserving every ownership tick.
- Service worker now fetches HTML network-first, so GitHub Pages updates cannot be hidden by an old cached index.html.
- Forces a service-worker update on load and reloads once when the new worker takes control.
- Retains v8 strict family validation, 1,200-variant sanity ceiling, and full collector-number formatting.
