# Recettes

{% for page in site.html_pages %}
  - [{{ page.title }}]({{ page.url | relative_url }})
  {{ page.description }}

{% endfor %}