# opportunities.com

Coming soon page for **opportunities.com** - a new job board built on real networks.
People find work there, and people open doors there.

## Stack

- Single static page, no build step: `index.html` + `assets/`
- Pixel art hero (true 384x216 pixel grid, rendered crisp via CSS pixelation)
- Vanilla JS email capture form; signups go to a private Google Sheet via a small
  Google Apps Script webhook (the script is intentionally not in this repo)

## Develop

Serve the repo root with any static server, e.g. `python3 -m http.server`.
The form endpoint lives in `FORM_ENDPOINT` at the bottom of `index.html`.

## Deploy

GitHub Pages, legacy build, serving from the repository root. Pushes to the
source branch redeploy automatically. Custom domain `opportunities.com`
is wired up after DNS is pointed at GitHub Pages.
