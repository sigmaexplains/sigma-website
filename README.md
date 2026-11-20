# sigma-website

The website for **Sigma Explains** (sigmaexplains.com): a STEM learning platform with an AI tutor that teaches
instead of giving answers. The site points learners to the app (app.sigmaexplains.com) and educators to Sigma Teach
(teach.sigmaexplains.com).

It's a static site: plain HTML and CSS with no build step and no dependencies.

```
index.html          the page
styles.css          all styles (responsive: phone, tablet, desktop; light and dark)
assets/favicon.svg  Σ icon
```

## Run it locally
Open `index.html` in a browser, or run:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Keep it current
- **Courses:** the Courses section lists what's live in the app and what's in development. Update it when a course
  is published (live catalogue: `GET /v1/courses` on the API).
- **Claims:** every number on the page has a source next to it. Keep it that way.

## Publish on GitHub Pages
1. In the repo, go to **Settings → Pages**.
2. Set **Source** to *Deploy from a branch*, then choose `main` and `/ (root)`.
3. To use your own domain, enter `sigmaexplains.com` under **Custom domain**, then point the domain's DNS to GitHub Pages.

Pushing to `main` publishes the site.
