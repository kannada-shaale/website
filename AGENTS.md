# AGENTS.md

This repository hosts the static website for **Nudi Kannada Shaale**.

## Site model

- The site is a plain static HTML site.
- The root `index.html` is a bilingual landing page with language choice.
- The English site lives under `en/`.
- The Kannada site lives under `kn/`.
- GitHub Pages publishes the repository root.

## File structure

- `index.html`
  Bilingual landing page with buttons for `English` and `ಕನ್ನಡ`
- `en/*.html`
  English pages
- `kn/*.html`
  Kannada pages
- `.github/workflows/deploy-google-sites-html.yml`
  GitHub Pages deployment workflow

## Content rules

- Keep English and Kannada site structure aligned.
- If you add a page in `en/`, add the corresponding page in `kn/` unless explicitly told not to.
- Keep the top-left brand linked to the language-specific home page:
  - English pages link brand to `en/index.html` relative as `index.html`
  - Kannada pages link brand to `kn/index.html` relative as `index.html`
- The main navigation should stay consistent across all pages in a language section.
- Current navigation model:
  - `Home` / `ಮುಖ್ಯಪುಟ`
  - `Curriculum` / `ಪಠ್ಯಕ್ರಮ`
  - `Resources` / `ಸಂಪನ್ಮೂಲಗಳು`
  - `Join Us` / `ನಮ್ಮೊಡನೆ ಸೇರಿ`
    - `Teachers` / `ಶಿಕ್ಷಕರು`
    - `Students` / `ವಿದ್ಯಾರ್ಥಿಗಳು`
    - `Collaborate` / `ಸಹಯೋಗ`

## Styling rules

- Each HTML page is self-contained and includes its own embedded `<style>` block.
- Do not introduce external CSS files unless explicitly requested.
- When changing layout or visual styles, keep the English and Kannada versions visually consistent.
- Prefer simple, readable, mobile-friendly styling.

## Language rules

- English copy should be warm, clear, and parent-friendly.
- Kannada copy should be natural and readable, not overly literal.
- Preserve meaning across languages even if wording differs slightly.
- Keep page titles, headings, and nav labels synchronized between `en/` and `kn/`.

## Current program constraints

- The school currently offers **Levels 1 through 4** only.
- Do not reintroduce `Level 5` unless explicitly requested.
- Level 4 includes the note that students may be ready to explore foreign language credit through local ISDs.

## Deployment rules

- The website is deployed through GitHub Pages using GitHub Actions.
- If new directories or files should trigger deploys, update `.github/workflows/deploy-google-sites-html.yml`.
- Keep `.nojekyll` at the repository root unless explicitly told to remove it.

## Editing guidance

- Prefer small, direct HTML edits.
- Keep links relative so the site works correctly on GitHub Pages project URLs.
- If renaming pages, update all affected links in both `en/` and `kn/`.
- If adding new sections to one language, mirror them in the other language unless asked otherwise.
