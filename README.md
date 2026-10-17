# Personal website

A personal website built with [Quarto](https://quarto.org/) and published with GitHub Pages.

## Requirements

- Git
- Quarto installed locally
- A GitHub repository

## Local preview

From the repository root (the folder containing `_quarto.yml`):

```bash
quarto preview
```

## Render the website

```bash
quarto render
```

The rendered website is written to `docs/`. Commit the updated `docs/` folder along with your source files if you publish through GitHub Pages using the `main` branch and `/docs` folder.

## Before publishing

1. Replace `Your Name` and the GitHub/LinkedIn placeholders in `_quarto.yml`.
2. Update the CV and About page.
3. Add your PDF CV at `assets/cv.pdf`, or remove the PDF link from `cv.qmd` until you have one.
4. Remove `draft: true` from posts when they are ready to publish.
5. Set GitHub Pages to **Deploy from a branch → main → /docs** in the repository's Settings → Pages.

## Add a post

Create a `.qmd` file in `posts/` with front matter such as:

```yaml
---
title: "A title for the essay"
description: "A one-sentence summary."
author: "Your Name"
date: 2026-12-01
categories:
  - Statistics
---
```

Then write the article below the front matter, run `quarto render`, and commit the changes.
