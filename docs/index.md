---
title: Welcome to Zip Captions
layout: default
---

Welcome to Zip Captions Helpdesk

{% for tutorials in site.tutorials %}
  <h2>
    <a href="{{ tutorials.url }}">
      {{ tutorials.title }}
    </a>
  </h2>
  <p>{{ tutorials.content | markdownify }}</p>
{% endfor %}
