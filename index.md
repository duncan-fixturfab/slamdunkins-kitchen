---
layout: default
title: Home
---

# Welcome to Slamdunkin's Kitchen

A collection of recipes, written simply.

## Recent Recipes

<ul class="recipe-list">
{% for recipe in site.recipes limit:5 %}
  <li>
    <h2><a href="{{ recipe.url | relative_url }}">{{ recipe.title }}</a></h2>
    <p class="date">{{ recipe.date | date: "%B %d, %Y" }}</p>
    {% if recipe.description %}
    <p>{{ recipe.description }}</p>
    {% endif %}
  </li>
{% endfor %}
</ul>

[View all recipes →](/recipes/)
