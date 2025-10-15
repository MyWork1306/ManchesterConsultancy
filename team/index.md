---
title: "Team"
layout: page
description: "Our expert team."
---

# Our Team

We are a small team of consultants with backgrounds in strategy, operations, finance and digital transformation.

<ul class="team-grid">
  {% for member in site.team %}
  <li class="team-card">
    <h3>{{ member.title }}</h3>
    <p class="muted">{{ member.position }}</p>
    <p>{{ member.content | strip_html | truncate:160 }}</p>
  </li>
  {% endfor %}
</ul>
