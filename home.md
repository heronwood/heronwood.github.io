---
title: Welcome to Heronwood Estates
---

{% assign pages=site.pages | where_exp: 'page', 'page.navigation != nil' | sort: 'navigation' %}

<ul class="pages">
{% for page in pages %}
  <li>
    <a href="{{ page.url }}" style="background-image: url({{ page.banner }});">{{ page.title }}</a>
    <p>{{ page.description }}</p>
  </li>
{% endfor %}
</ul>
