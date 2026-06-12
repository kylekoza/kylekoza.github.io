# kylekoza.github.io

Personal website for Kyle Koza — a cybersecurity leader specializing in
vulnerability management and application security. Built as a single static
page and hosted on GitHub Pages.

**Live site:** [www.kylekoza.com](https://www.kylekoza.com) · [kylekoza.github.io](https://kylekoza.github.io)

## Structure

| File       | Purpose                                              |
| ---------- | ---------------------------------------------------- |
| `index.html` | The entire page — markup and inline scripts        |
| `styles.css` | All styling (fonts, layout, hero vine, responsive) |
| `CNAME`      | Custom domain config for GitHub Pages              |

No build step, framework, or dependencies — just HTML and CSS. Fonts are loaded
from Google Fonts; everything else is self-contained.

## Developing locally

Open `index.html` directly in a browser, or serve the folder to mirror how
GitHub Pages serves it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

GitHub Pages serves the `master` branch from the repository root. Pushing to
`master` publishes the site:

```bash
git add index.html styles.css
git commit -m "Update site"
git push
```

### Custom domain

The `CNAME` file points the site at `www.kylekoza.com`. For that domain to
resolve, DNS must have a `CNAME` record for `www` pointing to
`kylekoza.github.io`.
