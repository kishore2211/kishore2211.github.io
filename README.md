# Kishore Yelchuri — Portfolio Website

Static personal portfolio site (plain HTML/CSS/JS, no build step).

```
index.html                     ← the whole site
assets/img/                    ← project images
assets/docs/Kishore_Yelchuri_Resume.pdf
assets/docs/Kishore_Yelchuri_Portfolio.pdf
```

## Host it free on GitHub Pages

### 1. Create the repository
1. Sign in at github.com → click **+** (top right) → **New repository**.
2. Name it exactly **`<your-username>.github.io`** (e.g. `ylnkishore.github.io`).
   This gives you the clean URL `https://<your-username>.github.io`.
3. Set it to **Public**, leave everything else unchecked, click **Create repository**.

### 2. Upload the files (no command line needed)
1. On the new repo page, click **uploading an existing file**.
2. Unzip the site folder on your computer, open it, select **everything inside it**
   (`index.html`, `README.md` and the `assets` folder) and drag it onto the page.
   Make sure `index.html` ends up at the top level of the repo, not inside a sub-folder.
3. Click **Commit changes**.

### 3. Turn on Pages
1. In the repo go to **Settings → Pages**.
2. Under **Build and deployment**: Source = **Deploy from a branch**, Branch = **main**, folder = **/ (root)** → **Save**.
3. Wait 1–2 minutes, refresh the page; it shows **"Your site is live at https://<your-username>.github.io"**.

### Alternative: command line
```bash
cd kishore-portfolio
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
git push -u origin main
```
Then do step 3 above.

## Updating later
- **New resume:** upload a new PDF with the *same name* (`assets/docs/Kishore_Yelchuri_Resume.pdf`)
  via **Add file → Upload files** — it replaces the old one and every link keeps working.
- **Edit text:** open `index.html` on GitHub, click the ✏️ pencil, edit, **Commit changes**.
- **Add a project:** in `index.html`, find `const projects = [` and copy one `{ ... },` block,
  then add its image to `assets/img/` using the same `id` as the file name (`my-project.jpg`).

Changes go live about a minute after each commit.

## Optional extras
- **Custom domain** (e.g. `kishoreyelchuri.com`): buy it from any registrar, then add it under
  Settings → Pages → Custom domain and follow GitHub's DNS instructions.
- **Add the link everywhere:** LinkedIn (Contact info → Website), your resume header, and your GitHub profile bio.
