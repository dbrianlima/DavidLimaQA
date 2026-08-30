# David Lima — QA Portfolio

A single-page portfolio site showcasing QA/test-automation skills, experience, and in-progress projects. Pure HTML/CSS — no build step, no dependencies to install.

## What's in this folder

```
qa-portfolio/
├── index.html   ← the entire site (content + styling)
└── README.md    ← this file
```

## Publish it with GitHub Pages

**Option A — a project site (repo can be named anything)**

1. Create a new repository on GitHub, e.g. `qa-portfolio`.
2. Upload `index.html` (and this `README.md` if you want) to the repo root — either drag-and-drop them in the GitHub web UI ("Add file → Upload files"), or via git:
   ```
   git init
   git add index.html README.md
   git commit -m "Add portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/qa-portfolio.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, select `main` and folder `/ (root)`, then **Save**.
6. GitHub will publish the site at:
   `https://<your-username>.github.io/qa-portfolio/`
   (takes a minute or two the first time)

**Option B — your main GitHub Pages site (root of your profile)**

If you want the site at `https://<your-username>.github.io/` directly (no `/qa-portfolio/` in the URL), name the repository exactly `<your-username>.github.io` instead, and upload `index.html` there. Pages auto-publishes from the `main` branch root for that repo — no extra settings needed.

## Before you publish

- **GitHub link**: the Contact section has a placeholder GitHub button. Open `index.html`, search for `add your username`, and replace that `<a>` tag's `href="#"` with your real GitHub URL (and update the visible text + remove the `is-placeholder` class so it stops looking dashed/greyed out).
- **Projects**: the Projects section is intentionally honest about status (`IN PROGRESS` / `PLANNED`). As you publish real repos, add a link on each `project-name` and flip the badge to reflect reality.
- **Content**: everything else (experience, skills, education, contact) reflects what you shared — update freely as things change.

## Local preview

No server needed — just open `index.html` directly in a browser, or run a quick local server from this folder:

```
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.
