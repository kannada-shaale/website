# Nudi Kannada Shaale Website

This repository now hosts a plain static HTML website for Nudi Kannada Shaale.

## Site Files

Main pages live at the repository root:

- `index.html`
- `curriculum.html`
- `resources.html`
- `teachers.html`
- `students.html`
- `collaborate.html`
- `level-1.html`
- `level-2.html`
- `level-3.html`
- `level-4.html`

Each page is self-contained with its own embedded CSS.

## GitHub Pages

This repo is configured to deploy directly to GitHub Pages with:

- `.github/workflows/deploy-google-sites-html.yml`

To enable it in GitHub:

1. Push this repo to the `main` branch.
2. Go to `Settings -> Pages`.
3. Set `Source` to `GitHub Actions`.

The site will publish from the repository root and use `index.html` as the homepage.

## Local Preview

Because this is a plain static site, you can preview it by opening `index.html` in a browser or by serving the folder with any simple static file server.
