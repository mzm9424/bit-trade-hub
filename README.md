# bit Trade net (BTN) — Static GitHub Deployment

A responsive static front-end implementation of the requested institutional cryptocurrency portal aesthetic.

## Files

- `index.html` — page shell
- `styles.css` — responsive dark institutional UI
- `app.js` — hash routing, UI state, login simulation, dashboard and withdrawal simulation
- `.github/workflows/deploy-pages.yml` — optional GitHub Pages deployment workflow

## Run locally

Open `index.html` in a browser, or serve the folder with any static server.

Example:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Login

Prototype credentials are intentionally client-side because this is a static front-end:

- Email: `Berginjoshua1@gmail.com`
- Password: `Thatguy12@`

Do not treat these credentials or the client-side session as real authentication.

## GitHub Pages

1. Create a public GitHub repository.
2. Upload these files to the repository root.
3. Push the `.github/workflows/deploy-pages.yml` workflow.
4. In GitHub, open **Settings → Pages** and select **GitHub Actions** as the source.
5. Push to `main`; the workflow publishes the static site.

## Security / financial disclaimer

This repository is a UI prototype. It does not custody cryptocurrency, connect to a blockchain, execute trades, process withdrawals, collect payments, or authenticate users securely.

The clearance step deliberately does **not** provide a real escrow/deposit wallet. It uses a non-functional simulation reference and QR-style graphic. A real application should never require a user to pay an arbitrary "clearance fee" to release funds without independently verifiable contractual and financial documentation.

For production authentication, use a server-side identity provider and keep secrets out of browser JavaScript.
