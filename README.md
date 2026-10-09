# Personal website — deploy with GitHub Pages

## Files
- `index.html` — the page (all content lives here)
- `style.css` — styling
- `cv.pdf` — **add your CV here** (the CV link points to it)
- `papers/priority-design-grant-funding.pdf` — **add the paper PDF here**, or point the link to SSRN/arXiv
- `photo.jpg` — optional headshot; uncomment the `<img>` line in `index.html`

## Before publishing, edit in `index.html`
1. Google Scholar and GitHub links (currently placeholders)
2. Email — swap to your Columbia address if you prefer
3. The abstract — it's a placeholder summary; paste in the paper's real abstract
4. The R&R line — remove it if you'd rather not list the journal yet

## Deploy (about 5 minutes)
1. Create a public GitHub repo named exactly `<your-username>.github.io`
2. Upload these files to the repo root (drag-and-drop on github.com works, or):
   ```
   git init && git add . && git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. In the repo: Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`
4. The site goes live at `https://<your-username>.github.io` within a minute or two

## Optional: custom domain (e.g. joejourden.com)
Buy the domain, add a file named `CNAME` containing `joejourden.com`, then set the domain under Settings → Pages and follow GitHub's DNS instructions.

## Updating
Edit `index.html`, commit, push. New papers: copy an `<article class="paper">` block.
