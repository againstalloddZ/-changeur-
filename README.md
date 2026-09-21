# Hyperliquid Scanner V3.3 — GitHub Pages V31

V31 is based on V30.

## Connector modes
- **Checkbox OFF:** keeps the V30 connector management unchanged.
- **Checkbox ON:** enables the new V31 connector geometry.

## V31 connector geometry
The requested percentages describe the **vertical distance travelled**, not the geometric length of the connector:
- **20%**: short vertical section from the exact x-axis graduation;
- **70%**: central section, vertical when the label is aligned, oblique when the label has been shifted;
- **10%**: short final vertical section into the exact center of the time label.

When the central section changes direction, smooth Bézier transitions are used so there are no sharp corners. The Bézier tangents are aligned with the vertical and oblique sections.

The V30 label placement is retained: each label is centered on its own graduation whenever possible; if the two labels would overlap, they are shifted as a pair and the connectors follow their final centers.
