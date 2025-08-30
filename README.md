# Background Remover (Client‑Only)

An in‑browser background removal tool that runs entirely on the client using MediaPipe Selfie Segmentation. No uploads or servers required — works great on GitHub Pages.

## Demo Path

- If this is served from a GitHub Pages site for your repo, open:
  - `https://<your-username>.github.io/<repo-name>/background-remover/`

## Links

- Portfolio: https://stiven-gjekaj.github.io/portfolio/

## Features

- Person background removal (portrait segmentation)
- Transparent or solid color background output
- Edge feathering (soften cutout)
- PNG download
- Mobile‑friendly quick actions interface
- Offline after initial load (assets are cached by your browser)

## Usage

1. Open `background-remover/index.html` in a modern browser (Chrome, Edge, Safari, Firefox).
2. Click “Upload” (or drop/paste an image) and then “Remove Background”.
3. Adjust Feather to smooth edges.
4. Pick “Transparent” or “Solid” and choose a color if desired.
5. Click “Download PNG”.

Tip: You can paste an image from your clipboard directly on the page (desktop).

## Mobile Interface

On phones and small tablets a simplified quick‑actions UI appears at the bottom:

- Upload, Remove, Download, Clear buttons
- Feather slider
- Background mode + color picker

The desktop controls remain available on larger screens with a two‑panel layout (controls + result).

## Limitations

- The included model is tuned for people (selfie segmentation). Results on non‑human objects vary.
- Very large images may be downscaled by the browser for performance.

## Customize Footer Signature

The footer shows a small signature. You can set it without editing code using a query parameter, and it will be remembered in `localStorage`:

- Example: `.../background-remover/?sig=Your%20Name`

Or edit the default text in `background-remover/index.html` (element with id `signature`).

## Deploy to GitHub Pages

1. Commit and push this folder to your GitHub repository.
2. In GitHub → Settings → Pages → Build and deployment:
   - Source: “Deploy from a branch”
   - Branch: your default (e.g., `main`), Folder: `/ (root)`
3. Wait for the build to finish, then open:
   - `https://<your-username>.github.io/<repo-name>/background-remover/`

## Tech Stack

- MediaPipe Selfie Segmentation (via jsDelivr CDN)
- Plain HTML/CSS/JS — zero build tools

## Privacy

All processing happens locally in the browser. Images never leave your device.
