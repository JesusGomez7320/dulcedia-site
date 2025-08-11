
# Dulce Día Cine — GitHub + Netlify Starter (Nguyen‑Style, with Video Lightbox)

This repo is a **static site** you can deploy free on Netlify. It includes:
- Responsive, light Nguyen-style layout
- SEO meta tags, Open Graph, JSON-LD
- Simple **lightbox** that plays **YouTube/Vimeo** when you click "View more"
- `/assets/images` folder for your thumbnails and about photo

## Quick Start
1. **Add images** to `assets/images/` (e.g., `sofia-matteo.jpg`). Keep them around **1600px wide**.
2. Open `index.html` and edit the **Portfolio** section: update the `<img src>` paths and the `data-video` to your **Vimeo** or **YouTube** link.
3. Edit copy in the **Hero**, **About**, **Packages**, and **Contact** sections.
4. Replace `og-cover.jpg` in `assets/images/` (recommended size: 1200x630).

## Deploying (GitHub → Netlify)
1. Create a GitHub repo and **upload** all files in this folder.
2. Go to Netlify → **Add new site** → **Import from Git** → connect your GitHub.
3. Select this repo. Build settings: **No build command** (it's static), **Publish directory:** `/`.
4. Netlify will deploy and give you a `.netlify.app` URL.

## Editing later
- Make changes locally or on GitHub’s web editor.
- **Push/commit**, Netlify auto-updates your site.

## SEO Checklist (after you have your domain)
- In `index.html`: update `<link rel="canonical" href="...">` to your final domain.
- In `robots.txt` and `sitemap.xml`: update the domain.
- Replace images with branded ones and write descriptive `alt` text.
- Keep images compressed (WebP/JPEG).

## Notes on Video
- Best practice: host films on **Vimeo** or **YouTube** and use `data-video` with the share URL.
- The lightbox converts links to embed forms automatically.
- For silent hero loops, use a short <video> with attributes `muted autoplay playsinline loop`.

