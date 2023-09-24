---
title: Knowledge Base
description: Search through known issues and workarounds
layout: default
---
<h2>Knowledge Base</h2>

Search through known issues and workarounds

<!-- Html Elements for Search -->
<div id="search-container">
Search our Knowledge Base:
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
  json: '/kb.json'
})
</script>

{% for kb in site.knowledge_base %}
  <h3>
    <a href="{{ kb.url | prepend: site.baseurl}}">
      {{ kb.title }}
    </a>
  </h3>
  <p>{{ kb.description | markdownify }}</p>
{% endfor %}