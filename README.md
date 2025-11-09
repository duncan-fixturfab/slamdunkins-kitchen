# Slamdunkin's Kitchen

A simple recipe website built with Jekyll and hosted on GitHub Pages.

## Features

- Clean, minimal design with white background and black text
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

This site is configured for GitHub Pages. To deploy:

1. Push changes to the repository
2. Go to repository Settings → Pages
3. Set Source to "Deploy from a branch"
4. Select your branch (e.g., `claude/recipe-posting-website-011CUwg3dFbDBhXnb1y76RxL` or `main`)
5. Click Save

GitHub Pages will automatically build and deploy your site.

## Structure

- `_config.yml` - Jekyll configuration
- `_layouts/` - HTML templates
- `_recipes/` - Recipe collection (Markdown files)
- `assets/css/` - Stylesheet
- `index.md` - Home page
- `recipes/index.md` - Recipe listing page
