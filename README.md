# Pallavi Jangid — Portfolio

A single-file, zero-dependency portfolio site. Left sidebar is fixed, right panel scrolls. Dark/light toggle included.

## Files
- `index.html` — the whole site. Edit this one file for all content changes.
- `resume.pdf` — (optional) drop your resume here so the Resume link works.

## Content you can edit quickly
Open `index.html` and update:

- **Name / role / phone / email** — top of the `<aside class="left">` block.
- **Manifesto line** — search for `class="manifesto"`. Alternates you can swap in:
  - "Directing attention. Shaping feeling." (current)
  - "Ideas with edges. Stories with soul."
  - "Crafting the feeling before the frame."
  - "Art direction as a point of view, not a polish."
- **Projects** — four `<article class="project">` blocks. Change the title, tag, year, and replace the `<div class="project-canvas">` with an `<img>` when you have real work:
  ```html
  <div class="project-canvas">
    <img src="images/campaign-01.jpg" alt="" style="width:100%;height:100%;object-fit:cover;">
  </div>
  ```
- **Fun / Play** — six `<div class="play-tile">` blocks at the bottom.
- **Social links** — update the `href="#"` values in the socials block.
- **Location label** — `<span id="loc">India</span>`.

## Deploy to GitHub Pages (free)

1. Create a new **public** repo on GitHub named something like `portfolio` (or `pallavijangid.github.io` for a root URL).
2. Upload `index.html` (and `resume.pdf` if you have one) to the repo root.
3. Repo → **Settings** → **Pages**.
4. Under "Build and deployment": **Source** = `Deploy from a branch`, **Branch** = `main`, folder = `/ (root)`. Save.
5. Wait ~1 minute. Your site goes live at `https://<your-username>.github.io/portfolio/`.

### When you buy a domain later
In the same Pages settings, add your custom domain (e.g. `pallavi.design`). Then at your domain registrar, add these DNS records:
- `A` record @ → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- `CNAME` record `www` → `<your-username>.github.io`

GitHub auto-issues an HTTPS cert. Done.

## Swapping in real images
Create a folder called `images/` in the repo and drop JPG/PNG/WebP files in. Aim for 1600 × 900 px for project canvases, 600 × 600 px for play tiles. Keep them under ~300KB each so the site stays fast.
