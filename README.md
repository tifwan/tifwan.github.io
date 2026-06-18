# Academic Personal Website

A lightweight, single-page academic homepage for your CV and biosketch. No build step, no dependencies — just static HTML/CSS hosted free on GitHub Pages.

## Files

```
academic-site/
├── index.html          # Your homepage (edit the text here)
├── assets/
│   ├── style.css       # Styling (colors via CSS variables at top)
│   ├── photo.jpg       # ← add your headshot
│   ├── CV.pdf          # ← add your CV
│   └── biosketch.pdf   # ← add your biosketch
└── README.md
```

## Quick deploy to GitHub Pages

You have two URL options. Choose one:

**Option A — `username.github.io` (root domain, recommended)**
1. Create a new repo named exactly `<your-username>.github.io` (e.g. `tifwan.github.io`).
2. Upload these files to the repo root.
3. Go to **Settings → Pages → Build and deployment**, set Source = `Deploy from a branch`, Branch = `main`, folder = `/ (root)`. Save.
4. Visit `https://<your-username>.github.io` (live in ~1 min).

**Option B — a project repo (e.g. `homepage`)**
1. Create any repo, upload the files.
2. Settings → Pages → Branch = `main`, `/ (root)`.
3. Visit `https://<your-username>.github.io/<repo-name>/`.

## Deploy from the command line

```bash
cd academic-site
git init
git add .
git commit -m "Initial academic homepage"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
git push -u origin main
```

Then enable Pages in repo Settings as above.

## What to edit

- **`index.html`** — replace the name, title, About text, research/teaching items, publications, email, and links. Search for `you@mail.cgu.edu.tw` and the GitHub URL.
- **`assets/photo.jpg`** — your headshot (square works best; ~400×400px).
- **`assets/CV.pdf`** and **`assets/biosketch.pdf`** — drop your actual PDFs in.
- **`assets/style.css`** — change the color theme by editing the `--accent` value at the top.

## Custom domain (optional)

If you own a domain, add a file named `CNAME` (no extension) containing just your domain (e.g. `wan.example.com`), then configure DNS per GitHub's docs.
