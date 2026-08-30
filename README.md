# Wifey's Pokémon Hunt — v8 Strict Family Audit

## Critical fix
- Core catalogue results are now accepted only when the actual Pokémon name/dex identity belongs to the selected evolution family.
- Broad/ignored API filters can no longer dump unrelated cards into a family.
- Example: Croconaw can never appear inside Growlithe / Arcanine.
- A second final validation pass removes any misfiled card before totals are calculated.
- Core cache bumped to v8, forcing a clean recount.
- Full collector-number formatting from v7 is retained (e.g. Growlithe 027/182).

Upload all files in this folder to the GitHub repo root and replace the existing files.
