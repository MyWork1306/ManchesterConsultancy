---
title: Services
layout: page
description: Our services.
---

# Services

We offer a broad range of services across strategy, operations, people and digital.

<ul class="services-list">
  {% for svc in site.services %}
  <li class="service-card">
    <h3><a href="{{ svc.url | relative_url }}">{{ svc.title }}</a></h3>
    <p>{{ svc.excerpt | strip_html | truncate:200 }}</p>
  </li>
  {% endfor %}
</ul>
