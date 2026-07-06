# Dr. Ashvani Kumar Patel — Faculty Profile Website

A single-page profile website for **Dr. Ashvani Kumar Patel**, Assistant Professor of Chemistry at Invertis University, Bareilly.

🔗 **Live demo (after deploy):** `https://<your-username>.github.io/<repo-name>/`

---

## 📁 What's in this repo

```
.
├── index.html   ← the full website (self-contained: HTML + CSS, no build step needed)
└── README.md    ← this file
```

`index.html` is completely self-contained — all styling is inline `<style>`, so there are no extra CSS/JS files to manage or paths to break.

---

## 🚀 Deploy with GitHub Pages (2 minutes, free)

1. **Create a new repository** on GitHub (e.g. `ashvani-kumar-patel`).
2. **Upload both files** (`index.html` and `README.md`) to the repo — either:
   - drag-and-drop them on the GitHub web UI ("Add file → Upload files"), or
   - via git:
     ```bash
     git init
     git add index.html README.md
     git commit -m "Add faculty profile website"
     git branch -M main
     git remote add origin https://github.com/<your-username>/<repo-name>.git
     git push -u origin main
     ```
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, select **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then click **Save**.
6. Wait ~1 minute — GitHub will publish the site at:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```
   (The exact URL is also shown at the top of the Pages settings screen once it's live.)

That's it — no build tools, no dependencies, no server required.

---

## ✏️ Editing the content

Everything is in `index.html`. Useful places to look:

| Section | What to update | Roughly around |
|---|---|---|
| Photo | `<img src="...">` in the `.portrait-frame` | top of `<body>` |
| Name / role / tagline | `<h1 class="name">`, `<p class="role">` | hero section |
| Key facts | `.facts` grid (designation, institution, email, articles) | `#about` section |
| Education | `.timeline` list items | `#education` section |
| Research areas | `.expertise-grid` cards + `.pillbar` tags | `#research` section |
| Publications | `.pub-list` items (title, authors, journal, DOI link) | `#publications` section |
| Social / contact links | `.social-row` cards | `#connect` section |

Since the whole page is one file, you can open `index.html` directly in a browser to preview changes before pushing.

---

## 🎨 Design notes

- Palette: warm light-orange background with a burnt-orange accent, built around CSS custom properties in `:root` — change these to re-theme the whole page in one place.
- Fully responsive: the hero, facts grid, expertise cards, and social links all reflow on mobile widths.
- No external fonts, images (other than the profile photo), or JS frameworks — fast to load, easy to host anywhere (GitHub Pages, Netlify, Vercel, or any static file host).

---

*Profile content compiled from Invertis University's official faculty listing, Google Scholar, and ResearchGate.*
