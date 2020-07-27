---
title: Events
---

<table class="events">
  {% for event in site.events reversed %}
    <tr>
      <td class="when">
        <div class="date">{{ event.date | date: '%B %e, %Y' }}</div>
        <div class="time">{{ event.date | date: '%l:%M%P' }}</div>
      </td>
      <td class="details">
        <div class="title">[{{ event.title }}]({{ event.url }})</div>
        <div class="location">{{ event.location }}</div>
      </td>
    </tr>
  {% endfor %}
</table>
