---
title: Help Articles
description: See the help documentation
layout: default
---
<h2>Help Articles</h2>

<!-- Html Elements for Search -->
<div id="search-container">
Search our help articles:
<input type="text" id="search-input" placeholder="search...">
<ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<script src="../search-script.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '/search.json'
})
</script>

{% for tutorial in site.tutorials %}
  <h3>
    <a href="{{ tutorial.url | prepend: site.baseurl}}">
      {{ tutorial.title }}
    </a>
  </h3>
  <p>{{ tutorial.description | markdownify }}</p>
{% endfor %}