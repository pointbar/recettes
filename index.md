---
title: Liste des recettes
page-type: summary
---

{% for page in site.html_pages %}
  {% unless page.page-type %}
  {:.summary}
  - [{{ page.title }}]({{ page.url | relative_url }})
  {% endunless %}
{% endfor %}
