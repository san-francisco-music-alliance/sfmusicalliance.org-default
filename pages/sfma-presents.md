---
layout: default
published: true
permalink: /sfma-presents/
title: SFMA Presents
color: '#C3573B'
order: 2
---

{% for n in site.sfmapresents  reversed %}
  {% if n.published == true  %}
<article>
<h4> {{ n.title }} </h4>
  <date>{{ n.date | date: '%B %d, %Y' }}</date>
  {{ n.content }}
</article>
  {% endif %}
{% endfor %}
