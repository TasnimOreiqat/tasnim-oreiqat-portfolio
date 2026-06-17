# Tasnim Oreiqat — Portfolio

A single-page portfolio site built with plain HTML, CSS, and JavaScript — no frameworks, no build step.

## Files

```
index.html      All page content and structure
style.css       Design tokens, per-project color themes, and animations
script.js       Nav menu, scroll-reveal, and presentation video play/pause
favicon.svg     Browser tab icon
images/         Every project image, shown directly inline (no click needed)
video/          The original presentation walkthrough video (autoplays)
files/          The original presentation PDF (downloadable from the site)
.nojekyll       Tells GitHub Pages to skip Jekyll processing
```

Every project has its own colorful, fully-visible image gallery built right
into its section — nothing is hidden behind a click. The presentation
project shows only its original video (autoplaying, muted, looping) with a
direct link to download the full PDF deck.


## Deploy on GitHub Pages

1. Create a new repository on GitHub (e.g. `portfolio`).
2. Push these files to the repository root (or to a `docs/` folder — just match the setting in step 4).
   ```
   git init
   git add .
   git commit -m "Portfolio site"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
   git push -u origin main
   ```
3. On GitHub, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to "Deploy from a branch," pick the `main` branch and the `/ (root)` folder, then save.
5. GitHub gives you a live URL within a minute or two, typically:
   `https://YOUR-USERNAME.github.io/YOUR-REPO/`

## After deploying

- Open `index.html` and update the `og:image` / `twitter:image` paths if you'd like a different social-share preview image.
- Replace any image in `images/` with an updated version using the same filename — no HTML changes needed.
- To use a custom domain, add a `CNAME` file with your domain name and configure DNS per GitHub's custom domain docs.

## Local preview

No server required — just open `index.html` directly in a browser. (For live-reload while editing, any simple local server works too, e.g. `python3 -m http.server`.)
