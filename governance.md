---
title: Governance
---

## Governing Documents

### Articles of Incorporation

Our [Articles of Incorporation]({% link governance/articles-of-incorporation.md %}) define the basic purpose and structure of our organization.

### By-Laws

Our [By-Laws]({% link governance/by-laws.md %}) dictate how our organization operates (meeting frequency, voting procedures, etc.).

### Covenants, Conditions, and Restrictions

Our [Covenants, Conditions, and Restrictions]({% link governance/covenants-conditions-and-restrictions.md %}) spell out the rights and obligations that the association has to its members and vice versa.

## Governing Bodies

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

## Frequently Asked Questions
