---
title: Latest Updates
description: See the latest features & updates
layout: default
---
<h1>Latest Updates</h1>

<h3>Keep track of our latest updates & features to learn what is new in each version:</h3>

<ul>
<ul>
  {% for post in site.posts %}
    <li>
      <p>{{ post.date | date: "%-d %B %Y" }}</p>
      <a href="{{ post.url | prepend: site.baseurl}}">{{ post.title }}</a>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
</ul>
