---
title: Team
layout: page
description: Meet our team.
---

# Our Team

<ul class="team-list">
{% for member in site.team %}
  <li class="team-card">
    <h3>{{ member.title }}{% if member.position %} - {{ member.position }}{% endif %}</h3>
    <p>{{ member.content | strip_html | truncate:200 }}</p>
  </li>
{% endfor %}
</ul>
