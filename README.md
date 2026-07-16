# Varshith Bala — Portfolio

A single-page portfolio site: dark, glassmorphic, animated data-pipeline hero, scroll reveals,
and sections for About, Skills, Experience, Projects (including live GitHub repos), a Roadmap
of upcoming projects, Certifications, Education, and Contact.

No build step — plain HTML/CSS/JS. Open `index.html` directly in a browser to preview locally.

## Files

```
portfolio/
├── index.html        # all content lives here
├── css/style.css      # design system + layout
├── js/main.js          # nav, scroll reveal, progress bar
└── netlify.toml        # Netlify config (optional but included)
```

## 1. Push to GitHub

You already have a `Varshith-Portfolio` repo. Two options:

**Replace its contents** (recommended, keeps the same URL):
```bash
git clone https://github.com/VarshithBala7/Varshith-Portfolio.git
cd Varshith-Portfolio
# delete old files, copy in index.html, css/, js/, netlify.toml from this build
git add .
git commit -m "Rebuild portfolio: dark glassmorphism redesign"
git push origin main
```

**Or start fresh in a new repo:**
```bash
cd portfolio
git init
git add .
git commit -m "Initial commit: portfolio site"
git branch -M main
git remote add origin https://github.com/VarshithBala7/YOUR-REPO-NAME.git
git push -u origin main
```

## 2. Deploy live on Netlify

1. Go to [app.netlify.com](https://app.netlify.com) → **Add new site → Import an existing project**.
2. Connect GitHub, pick your portfolio repo.
3. Build settings: leave **build command blank**, set **publish directory** to `.` (already set in `netlify.toml`).
4. Deploy. Netlify gives you a live URL immediately (e.g. `yourname.netlify.app`); you can add a custom domain later under **Domain settings**.

Every future `git push` to `main` auto-redeploys.

## 3. Things to personalize before/after pushing

- **GitHub repo cards** (in the "More on GitHub" block, `index.html`): four of your repos are
  linked with placeholder descriptions marked `— add description`. Swap in real one-liners for
  `AI-RESUME-SCREENER`, `scholarship-recommendation-assistant`, and `Portfolio`.
- **Resume download**: there's no resume file linked yet. Drop a PDF into the repo (e.g.
  `assets/Varshith-Bala-Resume.pdf`) and add a "Download Resume" button in the hero if you want one.
- **Favicon / social preview image**: none included yet — add a `favicon.ico` and an Open Graph
  image if you want nicer link previews when shared.
- **Roadmap section**: these are project ideas, not shipped work — update status tags
  (`Planning` → `In Progress` → done) or move them into Projects once built.
