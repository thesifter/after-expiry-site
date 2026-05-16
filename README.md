# After Expiry — Static Site

A minimal static site scaffold for the band **After Expiry**. Created 2025-09-13.

## Folder structure

```
after-expiry-site/
├── index.html
├── about.html               # optional
├── assets/
│   ├── css/
│   │   └── style.css
│   └── img/
│       └── logo.svg
├── robots.txt
├── sitemap.xml
└── README.md
```

## Local dev (no install needed)

Just open `index.html` in a browser — or run a tiny local server so relative links work nicely.

### Option A: VS Code Live Server (easy)

1. Open this folder in VS Code.
2. Install the **Live Server** extension (by Ritwick Dey).
3. Right‑click `index.html` → **Open with Live Server** (it will open on http://127.0.0.1:5500 or similar).

### Option B: Python built‑in server

From this folder, run one of the following and open http://localhost:5500 in your browser.

**macOS/Linux**

```bash
python3 -m http.server 5500
```

**Windows (PowerShell)**

```powershell
py -m http.server 5500
```

## Customize

- Edit titles, tagline, and sections in `index.html`.
- Replace the Bandcamp iframe src with your real embed.
- Swap social links in the **Social** section.
- Replace `assets/img/logo.svg` with your own logo.

## Next (optional)

When you're ready, init a git repo and push to GitHub Pages.
