---
title: Latest Updates
description: See the latest features & updates
layout: default
---
<h1>Latest Updates</h1>

<h3>Keep track of our latest updates & features to learn what is new in each version:</h3>

<ul>
{% for post in site.posts limit:5 %}  
  <li><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>  
{% endfor %} 
</ul>
