---
title: Governance
---

## Governing Documents

The following legal documents describe how our association is governed:

* Our [Articles of Incorporation](governance/articles-of-incorporation.md) define the basic purpose and structure of our association.
* Our [By-Laws](governance/by-laws.md) dictate how our association operates (meeting frequency, voting procedures, etc.).
* Our [Covenants, Conditions, and Restrictions](governance/covenants-conditions-and-restrictions.md) spell out the rights and obligations that the association has to its members and vice versa.

## Governing Bodies

The following elected bodies are responsible for governing our association.

### Board of Directors

{% for member in site.board_members %}
* {{ member.title }} - {{ member.name }} {% endfor %}

### Architectural Control Committee

{% if 0 < site.acc_members.size %}
  {% for member in site.acc_members %}
* {{ member.title }} - {{ member.name }} {% endfor %}
{% else %}
We do not currently have an elected Architectural Control Committee. As such, all architectural decisions fall to the [Board of Directors](#board-of-directors).
{% endif %}

## Treasurer's Reports

{% assign reports = site.static_files | where: 'report', true %}
{% for report in reports reversed %}
* [{{ report.basename}} ]({{ report.path }}){% endfor %}
