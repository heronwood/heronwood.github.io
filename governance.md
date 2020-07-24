---
title: Governance
---

## Governing Documents

### Articles of Incorporation

### By-Laws

### Covenants, Conditions, and Restrictions

## Governing Bodies

### Board of Directors

{% for member in site.board_members %}
* {{ member.title }} - {{ member.name }} {% endfor %}

### Architectural Control Committee

{% if site.acc_members %}
  {% for member in site.acc_members %}
* {{ member.title }} - {{ member.name }} {% endfor %}
{% else %}
We do not currently have an elected Architectural Control Committee. As such, all architectural decisions fall to the Board of Directors.
{% endif %}

## Frequently Asked Questions
