---
title: Latest Updates
description: See the latest features & updates
layout: default
---
<h1>Latest Updates</h1>

<h3>Keep track of our latest updates & features to learn what is new in each version:</h3>

<ul>
  {% for post of site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
