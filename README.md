[README.md](https://github.com/user-attachments/files/21908714/README.md)

# WILDeR Lab — Hugo + GitHub Pages Starter (PaperMod)

This is a ready-to-deploy Hugo site for the WILDeR Lab, set up for GitHub Pages + a custom domain (`wilderlab.org`).  
Theme: [PaperMod](https://github.com/adityatelange/hugo-PaperMod).

---

## Quick Start

1. **Create a new GitHub repo**, e.g. `wilderlab-site`.
2. **Download this starter** and extract it, then push all files to your repo.
3. **Add the PaperMod theme** (once, in your local clone):
   ```bash
   git submodule add https://github.com/adityatelange/hugo-PaperMod themes/PaperMod
   git commit -m "Add PaperMod theme"
   ```
   > Alternatively, vendor the theme by copying it into `themes/PaperMod`.

4. **Enable GitHub Pages**: Settings → Pages → Source: *GitHub Actions*.
5. The included GitHub Action will **build and deploy** on every push to `main`.
6. **Custom domain**: Settings → Pages → Custom domain = `wilderlab.org`.  
   Ensure your DNS has A records for `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`.  
   (Optionally set `www` CNAME → `YOUR_USERNAME.github.io`.)

## Local Development

1. Install [Hugo Extended](https://gohugo.io/installation/):  
   ```bash
   hugo version
   ```
2. Start the dev server:  
   ```bash
   hugo server -D
   ```
3. Open http://localhost:1313

## Structure

- `config.toml` — site config and menu
- `content/` — Markdown pages (edit these!)
- `static/CNAME` — sets the custom domain for Pages
- `.github/workflows/hugo.yml` — builds and deploys to `gh-pages`
- `assets/css/custom.css` — space for light style tweaks

## Next Steps

- Replace placeholder text in `content/` with your lab content.
- Add project subpages under `content/projects/`.
- Add lab members under `content/people/` (one `.md` per person).
- Wire deeper docs (protocols) to Notion or a private repo if needed.
