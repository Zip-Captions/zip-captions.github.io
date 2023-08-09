---
title: Welcome to Zip Captions
layout: default
---

Welcome to Zip Captions Helpdesk

{% for tutorial in site.tutorials %}
  <h2>
    <a href="{{ tutorial.url | prepend: site.baseurl}}">
      {{ tutorial.title }}
    </a>
  </h2>
  <p>{{ tutorial.description | markdownify }}</p>
{% endfor %}


<button name="button" onclick="https://www.zipcaptions.app">Go to Zip Captions Now</button>
