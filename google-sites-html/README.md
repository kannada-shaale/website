# Google Sites HTML Export

This folder contains a standalone HTML version of the site, separate from the Hugo build.

Included pages:

- `index.html`
- `curriculum.html`
- `resources.html`
- `contact.html`
- `level-1.html`
- `level-2.html`
- `level-3.html`
- `level-4.html`
- `level-5.html`

Shared styling lives in `styles.css`.

You can:

- host these files as a simple static site
- open them directly in a browser
- copy sections into Google Sites as a reference while rebuilding pages there

## GitHub Pages

This folder is now configured to deploy directly to GitHub Pages via:

- `.github/workflows/deploy-google-sites-html.yml`

It publishes the contents of `google-sites-html/` as the site root.

To enable it in GitHub:

1. Push the repository to GitHub on the `main` branch.
2. Open `Settings -> Pages`.
3. Set `Source` to `GitHub Actions`.
