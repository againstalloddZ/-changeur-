# Hyperliquid Scanner V3.3 — GitHub Pages V33

V33 is based on V32.

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
