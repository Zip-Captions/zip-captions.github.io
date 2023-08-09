---
title: Welcome to Zip Captions
layout: default
---
![Zip Captions logo](/assets/zip.jpg)

<h1>Welcome to Zip Captions Helpdesk</h1>

<h2>Help Articles</h2>
{% for tutorial in site.tutorials %}
  <h3>
    <a href="{{ tutorial.url | prepend: site.baseurl}}">
      {{ tutorial.title }}
    </a>
  </h3>
  <p>{{ tutorial.description | markdownify }}</p>
{% endfor %}


<button name="button" onclick="https://www.zipcaptions.app">Go to Zip Captions Now</button>
