---
layout: page
title: Blog
description: "Wszystkie wpisy na blogu Man of Iron, dokumentujące przygotowania do zawodów Ironman 70.3 w 2026 roku."
---

{% for post in site.posts %}
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
{% endfor %}

