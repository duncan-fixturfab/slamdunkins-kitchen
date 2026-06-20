# Slamdunkin's Kitchen

A simple recipe website built with Jekyll and hosted on GitHub Pages.

## Features

- Clean, modern design with a warm cream background and terracotta accents
- Recipe posts written in Markdown
- Simple navigation
- Mobile-friendly

## Adding New Recipes

To add a new recipe:

1. Create a new file in the `_recipes/` directory
2. Name it with a descriptive filename, e.g., `my-recipe-name.md`
3. Add frontmatter with recipe metadata:

```yaml
---
layout: recipe
title: Your Recipe Title
date: YYYY-MM-DD
description: A brief description of the recipe
servings: Number of servings
prep_time: Preparation time
cook_time: Cooking time
---
```

4. Write your recipe content in Markdown format

## Local Development

To run this site locally:

```bash
gem install bundler jekyll
jekyll serve
```

Then visit `http://localhost:4000`

## Deployment

This site auto-deploys to GitHub Pages via GitHub Actions
(`.github/workflows/deploy.yml`). Any push or merge to the `main` branch
triggers a build and deploy automatically.

One-time setup:

1. Go to repository Settings → Pages
2. Under "Build and deployment", set Source to **GitHub Actions**

After that, merging to `main` will build and publish the site with no
manual steps. You can also trigger a deploy manually from the Actions tab
("Deploy site to GitHub Pages" → Run workflow).

## Structure

- `_config.yml` - Jekyll configuration
- `_layouts/` - HTML templates
- `_recipes/` - Recipe collection (Markdown files)
- `assets/css/` - Stylesheet
- `index.md` - Home page
- `recipes/index.md` - Recipe listing page
