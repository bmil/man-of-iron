---
layout: page
title: Przepisy
---

<h1>Przepisy</h1>

<ul>
  {% for przepis in site.przepisy %}
    <li>
      <h2><a href="{{ przepis.url | relative_url }}">{{ przepis.title }}</a></h2>
    </li>
  {% endfor %}
</ul>

