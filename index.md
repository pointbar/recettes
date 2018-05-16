# Recettes

{% for page in site.html_pages %}
  - [{{ page.categorie }}]]({{ page.url | relative_url }})
{% endfor %}