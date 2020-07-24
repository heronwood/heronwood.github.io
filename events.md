---
title: Events
---

{% for event in site.events reversed %}
* [{{ event.url }}]({{ event.title }}) on {{ event.date | date: '%A, %B %e, %Y' }}
{% endfor %}
