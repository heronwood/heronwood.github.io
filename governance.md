---
title: Governance
description: Learn about the protections provided by our HOA and who our volunteers are.
banner: /images/20200510_174406.jpg
navigation: 2
---

## Governing Documents

The following documents describe how our association is governed:

* Our [Articles of Incorporation](governance/articles-of-incorporation.md) define the basic purpose and structure of our association.
* Our [By-Laws](governance/by-laws.md) dictate how our association operates (meeting frequency, voting procedures, etc.).
* Our [Covenants, Conditions, and Restrictions](governance/covenants-conditions-and-restrictions.md) spell out the rights and obligations that the association has to its members and vice versa.

## Boards and Committies

These fellow Heronwood Estates homeowners have been elected as volunteer members of the governing bodies that serve our association.

### Board of Directors

<ul class="profiles">
{% for member in site.board_members %}
  <li>
    <img src="{{ member.photo }}" alt="photo of {{ member.name }}" />
    <span class="title">{{ member.title }}</span>
    <span class="name">{{ member.name }}</span>
  </li>
{% endfor %}
</ul>

### Architectural Control Committee

{% if 0 < site.acc_members.size %}
  {% for member in site.acc_members %}
* {{ member.name }}{% endfor %}
{% else %}
We do not currently have an elected Architectural Control Committee. As such, all architectural decisions fall to the [Board of Directors](#board-of-directors).
{% endif %}

## Treasurer's Reports

<ul class="reports">
{% assign reports = site.static_files | where: 'report', true %}
{% for report in reports reversed %}
  <li><a href="{{ report.path }}">{{ report.basename }}</a></li>
{% endfor %}
</ul>
