# Shiva Sai — Portfolio

A single-page portfolio site styled as a live BI dashboard, built with plain HTML/CSS/JS (no build step required).

**Live demo:** _add your GitHub Pages link here after deploying, e.g._ `https://<your-username>.github.io/<repo-name>/`

---

## Deploy with GitHub Pages (free hosting)

### Option A — Using the GitHub website (no terminal needed)

1. Go to [github.com](https://github.com) and log in (or create a free account).
2. Click the **+** icon (top right) → **New repository**.
3. Name it something like `portfolio` or `shiva-sai-portfolio`. Keep it **Public**. Click **Create repository**.
4. On the new repo page, click **Add file → Upload files**.
5. Drag in `index.html` from this folder (and `README.md` if you want it visible on the repo).
6. Scroll down, click **Commit changes**.
7. Go to the repo's **Settings** tab → **Pages** (left sidebar).
8. Under **Build and deployment → Source**, choose **Deploy from a branch**.
9. Under **Branch**, select `main` and folder `/ (root)`, then click **Save**.
10. Wait 1–2 minutes, then refresh the page — GitHub will show your live URL:
    `https://<your-username>.github.io/<repo-name>/`

That's it — the site is now live and free, and updates automatically every time you upload a new `index.html`.

### Option B — Using git from your terminal

```bash
# 1. Create a new repo on GitHub first (via the website), then:
git init
git add index.html README.md
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main

# 2. Enable Pages
# Go to your repo on GitHub → Settings → Pages → Source: "Deploy from a branch"
# Branch: main, Folder: / (root) → Save
```

Your site will be live at:
`https://<your-username>.github.io/<repo-name>/`

---

## Using a custom domain (optional)

If you own a domain (e.g. `shivasai.dev`):
1. In your repo, add a file named `CNAME` containing just your domain, e.g. `shivasai.dev`.
2. In your domain registrar's DNS settings, add a `CNAME` record pointing to `<your-username>.github.io`.
3. In **Settings → Pages**, enter the custom domain and save. GitHub will auto-provision HTTPS.

---

## Editing the content

Everything lives in `index.html` — no separate data or build files. To update details:
- Contact info: search for `mailto:` and `tel:` in the file.
- Experience / skills / achievements: each section is clearly commented (`<!-- EXPERIENCE -->`, `<!-- SKILLS -->`, etc.).
- Colors: all defined as CSS variables at the top of the `<style>` block (`--bg`, `--teal`, `--amber`, etc.) — change these to re-theme the whole site.

No npm install, no build step — just open `index.html` in a browser to preview, or drag it directly into GitHub.
