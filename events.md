---
title: Events
---

{% for event in site.events reversed %}
* [{{ event.title }}]({{ event.url }}) on {{ event.date | date: '%A, %B %e, %Y at %l:%M%P' }}{% endfor %}
