---
title: Governance
---

## Governing Documents

The following legal documents describe how our association is governed.

### Articles of Incorporation

Our [Articles of Incorporation]({% link governance/articles-of-incorporation.md %}) define the basic purpose and structure of our association.

### By-Laws

Our [By-Laws]({% link governance/by-laws.md %}) dictate how our association operates (meeting frequency, voting procedures, etc.).

### Covenants, Conditions, and Restrictions

Our [Covenants, Conditions, and Restrictions]({% link governance/covenants-conditions-and-restrictions.md %}) spell out the rights and obligations that the association has to its members and vice versa.

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

## Frequently Asked Questions

### When is the next association meeting?

Our annual meeting occurs on a specified day in May at 7pm ([Article II, Section 1]({% link governance/by-laws.md %}#section-1-annual-meetings)). All association members will receive a notice (by mail and/or email) of the meeting at least 15 days in advance. Past and future [meetings can be found here]({% link events.md %}).
