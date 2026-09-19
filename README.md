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
