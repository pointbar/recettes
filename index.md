---
title: Sommaire
page-type: summary
---

{% for page in site.html_pages %}
  {% if !page.page-type %}
  {:.summary}
  - [{{ page.title }}]({{ page.url | relative_url }})
  {% endif %}
{% endfor %}
