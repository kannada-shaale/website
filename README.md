# ನಮ್ಮ ಕನ್ನಡ ಶಾಲೆ — Website

A Hugo-based website for ನಮ್ಮ ಕನ್ನಡ ಶಾಲೆ, hosting curriculum information, session notes, homework, and learning resources for Kannada families abroad.

## Project Structure

```
kannada-school/
├── content/                  # All markdown content
│   ├── _index.md            # Home page
│   ├── about/               # About the school
│   ├── curriculum/          # Curriculum pages (one per level)
│   │   ├── level-1/
│   │   ├── level-2/
│   │   ├── level-3/
│   │   ├── level-4/
│   │   └── level-5/
│   ├── classes/             # Session notes (updated weekly)
│   │   ├── level-1/
│   │   ├── level-2/
│   │   ├── level-3/
│   │   ├── level-4/
│   │   └── level-5/
│   ├── resources/           # Books, apps, links
│   ├── for-parents/         # Parent hub
│   └── showcase/            # Year-end showcase
├── static/
│   ├── presentations/       # Reveal.js presentation files
│   └── take-home-cards/     # PDF take-home cards
├── themes/kannada/          # Custom theme
│   ├── layouts/             # HTML templates
│   └── static/css/          # Stylesheet
├── .github/workflows/       # GitHub Actions auto-deploy
└── hugo.toml                # Site configuration
```

## Getting Started Locally

1. Install Hugo (version 0.123.7 or later, extended version):
   - Mac: `brew install hugo`
   - Windows: `choco install hugo-extended`
   - Linux: see https://gohugo.io/installation/linux/

2. Clone this repo and run:
   ```bash
   hugo server --buildDrafts
   ```

3. Visit `http://localhost:1313` to preview the site.

## Adding a New Session

Create a new markdown file in the relevant level folder:

```bash
# Example: Level 3, Session 5
touch content/classes/level-3/session-5.md
```

Use this template:

```markdown
---
title: "Session 5 — [Title]"
subtitle: "[Brief description]"
section_label: "Classes · Level 3"
level: "3"
session_number: 5
date: 2026-03-01
homework: true
---

## What We Covered

[Summary of the session]

### Vocabulary

| Kannada | Pronunciation | English |
|---------|--------------|---------|
| ಮನೆ | mane | home |

## Homework

1. [Task 1]
2. [Task 2]

## Notes for Parents

[Parent-facing notes]
```

## Deploying to GitHub Pages

1. Create a new GitHub repository
2. Push this project to the `main` branch
3. Go to **Settings → Pages → Source** and select **GitHub Actions**
4. The site will automatically build and deploy on every push to `main`
5. Update `baseURL` in `hugo.toml` to match your GitHub Pages URL:
   ```
   baseURL = "https://yourusername.github.io/kannada-school/"
   ```

## Updating Site Config

Edit `hugo.toml` to update:
- `baseURL` — your GitHub Pages URL
- `params.schoolYear` — current school year
- `params.contactEmail` — contact email
- `params.location` — your city

## Theme Customisation

The custom theme lives in `themes/kannada/`. The main stylesheet is at `themes/kannada/static/css/main.css`. Level colours, fonts, and spacing are all controlled via CSS variables at the top of that file.
