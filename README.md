# Publishing this site with GitHub Pages

This is a single static file (`index.html`), no build step needed.

## 1. Create a repository
1. Go to https://github.com/new
2. Name it `rikkeyeh.github.io` (using your exact GitHub username) if you want it at the root domain, or any name (e.g. `my-site`) if you're fine with a `/repo-name/` path.
3. Set it to **Public**, then create it.

## 2. Upload the file
- Easiest: on the repo page, click **Add file → Upload files**, drag in `index.html`, and commit.
- Or via command line:
  ```bash
  git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
  cp index.html YOUR-REPO/
  cd YOUR-REPO
  git add index.html
  git commit -m "Add site"
  git push
  ```

## 3. Turn on GitHub Pages
1. In the repo, go to **Settings → Pages**.
2. Under "Build and deployment", set **Source** to `Deploy from a branch`.
3. Set branch to `main` and folder to `/ (root)`, then **Save**.
4. Wait 1–2 minutes. Your site will be live at:
   - `https://YOUR-USERNAME.github.io/` (if repo is named `YOUR-USERNAME.github.io`), or
   - `https://YOUR-USERNAME.github.io/YOUR-REPO/` (any other repo name)

## Making edits later
Edit `index.html` directly in GitHub (pencil icon on the file) or re-upload after editing locally — Pages redeploys automatically on every push to the branch.
