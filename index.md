---
title: Liste des recettes
page-type: summary
---
{% assign sorted-pages = site.html_pages | sort: 'title' %}
{% for page in sorted-pages %}
  {% unless page.page-type %}
  <article class="summary">
    <h3><a href="{{ page.url | relative_url }}">{{ page.title }}</a></h3>
    <p>{{ page.description }}</p>
  </article>
  {% endunless %}
{% endfor %}
