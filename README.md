# Hyperliquid Scanner V3.3 — GitHub Pages

This edition is based on the supplied scanner frontend and removes the Netlify
Function dependency. The browser calls the Hyperliquid Info API directly.

## Deploy

1. Create a GitHub repository.
2. Upload the contents of this folder to the repository root.
3. Push to the `main` branch.
4. In GitHub: Settings → Pages → Source: GitHub Actions.
5. The workflow deploys `index.html` automatically after each push.

## Important

The scanner uses the Hyperliquid public Info endpoint:
`https://api.hyperliquid.xyz/info`

No API key is required for these public market-data calls.


## V3.3 display updates
- Ranking count no longer mentions "2 maximum par perp".
- Ranking vignette displays movement % × max leverage as a positive gain with `+`, green for upward moves and red for downward moves.
- Max leverage is displayed directly beside the perp name.
- Times are always shown before dates.
- Dates are omitted when the movement starts and ends on the same calendar day.
- Chart start/end time labels are drawn inside the chart.

- Ranking arrows are now placed after the coin and max leverage.
- Winner header uses the same coin + leverage + arrow arrangement.
- Ranking and winner display both the leveraged score and the raw movement percentage without verbose labels.
- Main chart now uses OHLC candlesticks.
- Start/end times are also shown on analog clocks with minute graduations and no seconds hand.
