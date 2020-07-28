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

## Frequently Asked Questions

### When is the next association meeting?

Our annual meeting occurs on a specified day in May at 7pm ([Article II, Section 1](governance/by-laws.md#section-1-annual-meetings)). All association members will receive a notice (by mail and/or email) of the meeting at least 15 days in advance. Past and future [meetings can be found here](events.html).

### What actions require approval from the Architectural Control Committee or Board of Directors?

Per our CC&Rs ([Article V, Section 2](governance/covenants-conditions-and-restrictions.md#section-2-approval-required)), the following actions require approval:

> 1. Clearing of any lot.
> 2. Removal any growing tree larger than 10" at its base.
> 3. Construction of any building or structure, including outbuildings, fences, and walls.
> 4. Alteration of the exterior of any building or improvement, including any change in exterior color and type of roof other than architectural grade shingles, shakes, tile or high-grade metal.
> 5. Excavation, grading or removal of dirt.
> 6. Any alteration of the natural drainage on a lot.
> 7. Installation of exterior lighting which is visible from any street, open space, or house within the property. 
> 8. Removal of vegetation of any kind from screening easements along Briarwood Lane or the screening easements along the rear lot lines of those residential lots numbered 27 through 41, inclusive, except the vegetation removal required in the interest of safety or necessitated by the emplacement of drainage facilities or other common utilities. 
> 9. Fencing of any kind within the screening easements or common areas along Brianvood Lane or the screening easements along the rear lot lines of those residential lots numbered 27 through 41, inclusive.

Additionally, according to [Article VII, Section 16](governance/covenants-conditions-and-restrictions.md#section-16):

> No changes in landscaping, nor removal or trimming of trees, lawns, or shrubs will be permitted within the common areas without written authorization of the Board or the Architectural Control Committee.

### How much are our HOA fees, and when are they due?

Heronwood Estates has an annual fee (also known as an *annual assessment*) of $120 per lot per year. The assessment is due on January 15th each year and must be paid within 30 days.
