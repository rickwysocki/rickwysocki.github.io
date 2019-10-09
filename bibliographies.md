---
title: Bibliographies
layout: default
description: Bibliographies assembled by Rick Wysocki over the course of his research.
image: assets/images/rickapril.jpg
order: 3
---

## Bibliographies

<ul>
{% for bibliography in site.bibliographies %}
    <li><a href="{{ bibliography.url }}">
      {{ bibliography.title }}
    </a></li>
{% endfor %}
</ul>
