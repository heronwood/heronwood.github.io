---
title: Frequently Asked Questions
---

## Questions

{% for question in site.faqs %}
* [{{ question.title }}](#{{ question.title | slugify }}){% endfor %}

Have another question that isn't answered here? Try [reading our governing documents](governance.md#governing-documents) or [contacting the Board of Directors](contact.md).

{% for question in site.faqs %}
## {{ question.title }}

{{ question.content }}
{% endfor %}
