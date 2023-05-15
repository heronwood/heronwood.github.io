---
title: Governance
description: Learn about the protections provided by our HOA and who our volunteers are.
banner: /images/20200510_174406.jpg
navigation: 2
---

<div class="notice">
  <p>In May of 2023, the Heronwood Estates HOA Board sent out a survey about changes to the annual assessment. <a href="{% link misc/2023-assessment-survey-results.md %}">View the results.</a></p>
</div>

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
    <img src="{{ member.photo | escape }}" alt="photo of {{ member.name | escape }}" />
    <span class="title">{{ member.title | escape }}</span>
    <span class="name">{{ member.name | escape }}</span>
  </li>
{% endfor %}
</ul>

### Architectural Control Committee

{% if 0 < site.acc_members.size %}
<ul class="profiles">
  {% for member in site.acc_members %}
  <li>
    <img src="{{ member.photo | escape }}" alt="photo of {{ member.name | escape }}" />
    <span class="title">{{ member.title | escape }}</span>
    <span class="name">{{ member.name | escape }}</span>
  </li>
  {% endfor %}
</ul>
{% else %}
We do not currently have an elected Architectural Control Committee. As such, all architectural decisions fall to the [Board of Directors](#board-of-directors).
{% endif %}

### Landscaping Committee

The Landscaping Committee is comprised of homeowner volunteers who help maintain and beautify the HOA common areas or "Open Spaces."

Meetings and work parties are on an ad hoc basis, depending on weather and committee volunteers' availability.

Upcoming projects - Clean-up “Open Spaces” including weeding, removing debris and invasive ivy/blackberries and, in some areas, restoring native vegetation:
* Along 38th Avenue
* Along Briarwood Lane
* Pond area
* 30' to 50' neighborhood perimeter (likely starting from 38th to pond area)

Recent accomplishments:
* Improved landscaping on each side of lower sign (removed invasive plants; planted native plants)
* (Ongoing) Weed and clean up around upper and lower sign areas
* (Ongoing) Weed sidewalk strip
 

If interested in participating or learning more, [contact the board](contact).

## Records

### Meeting Minutes

{% assign meetings = site.events | where: 'tags', 'meeting' | where_exp: 'item', 'item.content != ""' | reverse %}

{% for meeting in meetings -%}
* [{{ meeting.title | escape }}]({{ meeting.url }}) ({{ meeting.date | date: '%B %e, %Y' }})
{% endfor %}

### Treasurer's Reports

<ul class="reports">
{% assign reports = site.static_files | where: 'report', true %}
{% for report in reports reversed %}
  <li><a href="{{ report.path | escape }}">{{ report.basename | escape }}</a></li>
{% endfor %}
</ul>
