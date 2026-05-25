# BCIS Alumni Website V2 — Design Review

Static HTML mockups for admin review. Open `index.html` for a hub that links to every page.

## Project structure

```
AlumniWebsiteV2Design/
├── index.html                 # Review hub (start here)
├── design-v1/                 # Version 1 mockups
│   └── homepage.html
├── design-v2/                 # Version 2 mockups
│   ├── homepage.html
│   └── gallery.html
└── functional-updates/        # New feature pages
    ├── alumni-pass.html
    ├── directory.html
    └── mentor.html
```

## Local preview

From this folder, run a static file server (required for pages that load external scripts or assets over HTTP):

```bash
cd AlumniWebsiteV2Design
python3 -m http.server 8080
```

Then open [http://localhost:8080](http://localhost:8080).

To share on your LAN, use your machine’s IP instead of `localhost` (e.g. `http://192.168.1.10:8080`).

## Hosting

Upload the entire folder to any static host (Netlify, Vercel, GitHub Pages, S3, etc.). Set the site root to this directory; `index.html` is the entry point.

## Notes

- All pages are self-contained HTML with inline CSS (no build step).
- Some pages load fonts and libraries from CDNs; an internet connection is needed for full styling and behavior (e.g. Directory map).
- For internal review only.
