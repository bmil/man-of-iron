---
layout: page
title: Blog
description: "Wszystkie wpisy na blogu Man of Iron, dokumentujące przygotowania do zawodów Ironman 70.3 w 2026 roku. Trening, odżywianie, sprzęt, motywacja."
---

{% seo %}

# Wszystkie wpisy na blogu

<p>Znajdziesz tu pełną listę wpisów dokumentujących moją drogę do Ironman 2026: treningi, sprzęt, odżywianie, wyzwania i postępy.</p>

<ul>
{% for post in site.posts %}
  <li>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
    <small>{{ post.date | date: "%d.%m.%Y" }}</small>
  </li>
{% endfor %}
</ul>
