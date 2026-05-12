# ಹೊಸ ಚಿಗುರು Website

This repository now hosts a plain static HTML website for ಹೊಸ ಚಿಗುರು.

## Site Files

The repository now has:

- a bilingual landing page at `index.html`
- an English site under `en/`
- a Kannada site under `kn/`

Main English pages:

- `en/index.html`
- `en/curriculum.html`
- `en/resources.html`
- `en/teachers.html`
- `en/students.html`
- `en/collaborate.html`
- `en/level-1.html`
- `en/level-2.html`
- `en/level-3.html`
- `en/level-4.html`

Main Kannada pages:

- `kn/index.html`
- `kn/curriculum.html`
- `kn/resources.html`
- `kn/teachers.html`
- `kn/students.html`
- `kn/collaborate.html`
- `kn/level-1.html`
- `kn/level-2.html`
- `kn/level-3.html`
- `kn/level-4.html`

Each page is self-contained with its own embedded CSS.

## GitHub Pages

This repo is configured to deploy directly to GitHub Pages with:

- `.github/workflows/deploy-google-sites-html.yml`

To enable it in GitHub:

1. Push this repo to the `main` branch.
2. Go to `Settings -> Pages`.
3. Set `Source` to `GitHub Actions`.

The site will publish from the repository root and use `index.html` as the bilingual homepage.

## Local Preview

Because this is a plain static site, you can preview it by opening `index.html` in a browser or by serving the folder with any simple static file server.
