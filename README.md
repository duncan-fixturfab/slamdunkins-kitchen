# Slamdunkin's Kitchen

A simple recipe website built with Jekyll and deployed on Vercel.

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
bundle install
bundle exec jekyll serve
```

Then visit `http://localhost:4000`

## Deployment

This site is deployed on [Vercel](https://vercel.com). Build settings live
in `vercel.json` (framework preset `jekyll`, building to `_site`), and the
Ruby/Jekyll dependencies are pinned in the `Gemfile`.

One-time setup:

1. In the Vercel dashboard, **Add New… → Project** and import this
   GitHub repository.
2. Vercel reads `vercel.json` automatically — no build settings to change.
3. Click **Deploy**.

After that, Vercel deploys automatically on every push:

- Pushes/merges to the production branch (`main`) publish to production.
- Pull requests get their own preview deployment.

## Structure

- `_config.yml` - Jekyll configuration
- `_layouts/` - HTML templates
- `_recipes/` - Recipe collection (Markdown files)
- `assets/css/` - Stylesheet
- `index.md` - Home page
- `recipes/index.md` - Recipe listing page
