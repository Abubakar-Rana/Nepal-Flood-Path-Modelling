# Trishuli–Narayani Flood Model

Terrain flow-routing model of the 26 August 2026 Trishuli glacial-lake outburst,
from the Nepal–China border to the Gandak barrage at the Indian frontier.

The site is a single page with three tabs:

| Tab | File | What it is |
|---|---|---|
| 2D spread map | `pages/map-2d.html` | Zoomable animated map of the flood spreading across the floodplain |
| 3D terrain | `pages/map-3d.html` | WebGL terrain view of the same model (uses three.js from cdnjs) |
| Full report | `pages/report.html` | Method, validation and exposure |

Each tab can be linked to directly: `index.html#2d`, `#3d`, `#report`.

## Publish on GitHub Pages

```bash
git init
git add .
git commit -m "Trishuli flood model site"
git branch -M main
git remote add origin https://github.com/Abubakar-Rana/Nepal-Flood-Path-Modelling.git
git push -u origin main
```

Then on GitHub, go to **Settings → Pages → Build and deployment**, set
**Source: Deploy from a branch**, and pick **Branch: `main`** and folder **`/ (root)`**.
The site will be at `https://abubakar-rana.github.io/Nepal-Flood-Path-Modelling/` a minute later.

## Run locally

Open `index.html` directly, or serve the folder:

```bash
python -m http.server 8000
# http://localhost:8000
```

The pages are self-contained (data and images are embedded), so no build
step is needed. The only external resources are Google Fonts and three.js.
