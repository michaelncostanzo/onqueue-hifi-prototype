# OnQueue — High-Fidelity Interactive Prototype

Self-contained, clickable prototype of **OnQueue**, a production-scheduling app for a
print & embroidery shop. Static HTML/CSS/JS, no build step, no dependencies (fonts load
from Google Fonts).

## What's here

- `index.html` — landing / chooser page. Two buttons: **Open desktop prototype** and
  **Open phone prototype**.
- `HiFi_Desktop.html` — the desktop board (production board, Add-Job drawer with a
  setup-aware estimate, preview-and-commit "ripple", job detail, edit, notifications,
  hover-zoom explainers).
- `HiFi_Phone.html` — the phone build of the same product (method/machine switching,
  day strip, job detail, Add-Job estimate, long-press reorder, notifications).

## Run locally

Open `index.html`, or serve the folder:

```bash
npx serve .
# or
python3 -m http.server 8000
```

## Deploy (static site)

Plain static site — no framework or build. On Vercel, deploy with Framework preset
**Other**, no build command, output directory **.** (root `index.html` is the landing page).
