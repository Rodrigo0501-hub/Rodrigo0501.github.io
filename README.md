# Rodrigo Noriega — Portfolio Site

A single-file portfolio site (HTML/CSS/JS, no build step) styled as an engineering drawing set — each section is a numbered "sheet," with skills laid out as a Bill of Materials and projects as detail drawings.

## Files
- `index.html` — the entire site (HTML + CSS + JS in one file)
- `rodrigo-headshot.png` — your headshot, referenced by the cover sheet. Keep it in the same folder as `index.html` (same relative path), or update the `src` in the `id-frame` block if you rename/move it.

## Deploy on GitHub Pages (free, gives you a `github.io` URL)

**Option A — personal site at `yourusername.github.io`**
1. Create a new GitHub repo named exactly `yourusername.github.io` (replace with your actual GitHub username).
2. Upload `index.html` **and** `rodrigo-headshot.png` to the root of that repo (drag-and-drop on github.com works, or use git push).
3. Go to the repo's **Settings → Pages**. Under "Build and deployment," set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. Wait 1–2 minutes, then visit `https://yourusername.github.io`.

**Option B — project site at `yourusername.github.io/portfolio`**
1. Create a repo with any name, e.g. `portfolio`.
2. Upload `index.html` and `rodrigo-headshot.png` to the root.
3. Settings → Pages → Source: Deploy from a branch → `main` → `/ (root)` → Save.
4. Visit `https://yourusername.github.io/portfolio`.

### Using git from the command line instead
```bash
git init
git add index.html rodrigo-headshot.png README.md
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/yourusername/your-repo-name.git
git push -u origin main
```
Then enable Pages as described above.

## Customizing later
- All content (text, links, dates) lives directly in `index.html` — search for the section you want (e.g. `id="projects"`) and edit the text between the tags.
- Colors and fonts are defined as CSS variables at the top of the `<style>` block (the `:root { ... }` section), so you can retheme by changing a handful of hex values.
- To add a downloadable resume: drop a `resume.pdf` file next to `index.html` in the repo, then add a link such as `<a class="btn btn--ghost" href="resume.pdf">Resume</a>` in the Contact section.
- A custom domain (instead of `github.io`) can be added later via Settings → Pages → Custom domain.
