---
title: Liste des recettes
page-type: summary
---

{% assign sorted-pages = site.html_pages | sort: 'title' %}
{% for page in sorted-pages %}
  {% unless page.page-type %}
  {:.summary}
  - [{{ page.title }}]({{ page.url | relative_url }})
  {% endunless %}
{% endfor %}
