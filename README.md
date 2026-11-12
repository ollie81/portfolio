# Portfolio

A static, dependency-free portfolio site: one HTML page, one stylesheet, one small script, and optimized WebP screenshots. It has no build step, framework, tracking or paid service.

```
index.html        page content (projects, contact section, metadata)
styles.css        dark theme, responsive layout, animations
main.js           mobile menu, reveal-on-scroll, footer year (the page also works without JS)
favicon.svg
404.html
robots.txt        allows all crawlers, points to the sitemap
sitemap.xml       single-page sitemap with the deployed URL
OUTREACH-KIT.md   bio, project links and message templates for sharing the work (not part of the site)
assets/og-image.png        1200×630 social sharing image (made from real VIYO screenshots)
assets/img/*.webp          screenshots, each in 2 sizes for srcset
```

## Run locally

```bash
python3 -m http.server 8080
# open http://localhost:8080
```

You can use any static file server (`npx serve .` works too).

## Before you publish: things to edit

1. **Contact details.** The public contact email is `olli1234x@gmail.com`. It appears in the Contact section of `index.html` as a "Contact me" button and a clickable `mailto:` link. To change it, edit both `mailto:` links there.
2. **Domain.** The site URL `https://portfolio-kappa-ebon-cjtxzh45c6.vercel.app/` is set in the `<head>` of `index.html` (canonical, `og:url`, `og:image`, `twitter:image`). If you move to a custom domain, update those 4 places. Social previews need an absolute image URL.
3. **Live product links.** The site links to VIYO (`https://viyo.site/app`), Ollie (`https://www.ourollie.space`), Ollieen (`https://www.ollieen.com`) and Day-2 (`https://day-2-steel-eight.vercel.app`). If a URL changes, update it in `index.html` and `OUTREACH-KIT.md`.

## Deploy for free

All of these options are free for a static site. Pick one.

### Option A: GitHub Pages (simplest, since the code is already on GitHub)
1. Merge this branch into `main` (or the repo's default branch).
2. On GitHub, open the repository's **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*. Choose the branch `main` and the folder `/ (root)`, then click **Save**.
4. After about a minute the site is live at `https://ollie81.github.io/portfolio/`. All paths are relative, so the site works under that sub-path.
5. Put that URL into the `<head>` (see step 2 above), then commit.

### Option B: Netlify
1. Go to app.netlify.com, choose **Add new site → Import an existing project**, and pick this repository.
2. Leave **Build command** empty. Set **Publish directory** to `.`
3. Click **Deploy**. Netlify serves `404.html` automatically.

### Option C: Vercel / Cloudflare Pages
- **Vercel:** import the repo and set Framework preset to *Other*. Leave the build command empty and set the output directory to `.`
- **Cloudflare Pages:** connect the repo, leave the build command empty and set the output directory to `/`.

You can attach a custom domain for free on any of these hosts. You only pay for the domain registration itself.

## Content sources

Every project description comes from the project's own repository README or code. The VIYO screenshots are the real screenshots committed to `ollie81/Viyo-`; the phone status bar and system navigation bar are cropped off. The Village screenshot comes from `ollie81/THE-VILLAGE-THAT-REMEMBERS/docs/screenshots`. The Ollie, Ollieen and Day-2 images are real captures of each app's public landing page (Ollie web `/`, Ollieen `/welcome`, Day-2 `/` in dark mode). Each app was run locally from its own repository and captured at 1280×720. No login, account or user data appears in them. To replace one, drop a 16:9 WebP into `assets/img/` and update the matching `<img>` in `index.html`.
