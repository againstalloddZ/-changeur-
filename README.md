# Hyperliquid Scanner V3.4 — GitHub Pages V34

V34 is based on V33.

## Changes in V34
- New "Liste des perps" controls: the perps list can now hide the least liquid markets.
- Open interest and 24h volume are fetched from the Hyperliquid `metaAndAssetCtxs` endpoint during diagnostics.
- "Exclure les moins liquides" removes the N perps with the weakest open interest (notional) and the N perps with the weakest 24h volume. N is adjustable for each criterion (default: 30 / 30).
- The list can be sorted alphabetically or by 24h volume (descending), and filtered down to a single starting letter ("Toutes" shows every letter).
- The list now shows the coin name and its maximum leverage instead of the compass angle; the angle is still available in the tooltip of each row and on the compass itself.
- The compass, the rays and the scan itself are unchanged: the liquidity filter only affects the perps list. Pinning a perp from the list still highlights its ray.
- Every setting (filter on/off, both exclusion counts, sort order, selected letter) is remembered in `localStorage`.

## Changes in V33
- Direction text in the titles now uses `LONG` for upward movements and `SHORT` for downward movements instead of arrows.
- The sign `+`/`-` was removed from the percentage multiplied by maximum leverage; the leveraged score is displayed as a plain percentage.
- The connector checkbox still selects the experimental/new connector system only when checked.
- The unchecked branch keeps the existing V30/V27 reference behavior unchanged.
- When the new connector system is checked, each time label is first centered individually on its exact chart graduation. Labels are moved only when they would overlap; the algorithm first attempts an equal translation and uses symmetric separation only as a last resort.
- The checked connector geometry keeps the requested 20% / 70% / 10% vertical-height structure, with smooth tangent Bézier transitions and a dominant diagonal section when labels are displaced.
- Analog clock hands remain slightly longer than V32.
- Existing explanatory comments around connector geometry have been kept and expanded for manual editing.

## Deployment
Use the included GitHub Pages workflow from `.github/workflows/pages.yml`.
