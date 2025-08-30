# Background Remover

An in‑browser background removal tool that runs entirely on the client using MediaPipe Selfie Segmentation. No uploads or servers required.

## Features

- Person background removal (portrait segmentation)
- Transparent or solid color background output
- Edge feathering (soften cutout)
- PNG download
- Mobile‑friendly quick actions interface
- Offline after initial load (assets are cached by your browser)

## Usage

1. Click “Upload” (or drop/paste an image) and then “Remove Background”.
2. Adjust Feather to smooth edges.
3. Pick “Transparent” or “Solid” and choose a color if desired.
4. Click “Download PNG”.

Tip: You can paste an image from your clipboard directly on the page (desktop).

## Mobile Interface

On phones and small tablets a simplified quick‑actions UI appears at the bottom:

- Upload, Remove, Download, Clear buttons
- Feather slider
- Background mode + color picker

## Limitations

- The included model is tuned for people (selfie segmentation). Results on non‑human objects vary.
- Very large images may be downscaled by the browser for performance.

## Tech Stack

- MediaPipe Selfie Segmentation (via jsDelivr CDN)
- Plain HTML/CSS/JS — zero build tools

## Privacy

All processing happens locally in the browser. Images never leave your device.
