---
title: Welcome to Zip Captions
layout: default
---
![Zip Captions logo](/assets/zip.jpg)

<h1>Welcome to Zip Captions Helpdesk</h1>

Zip Captions is a browser based live captioning tool. Zip Captions main features are:

- Free!
- Accurate transcription
- Speech pause recognition creating a new line with pauses for more natural transcription
- Customisable themes and settings
- Transcription in English, French, Spanish, German and Italian
- Multi device support
- More features coming soon

<a href="https://www.zipcaptions.app">Go to Zip Captions Now</a>

<hr>
<h2>Most Recent Updates</h2>
<ul class="entries">
   {% for post in site.posts limit:2 %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}
</ul>

<hr>
<h2>Help Articles</h2>
{% for tutorial in site.tutorials %}
  <h3>
    <a href="{{ tutorial.url | prepend: site.baseurl}}">
      {{ tutorial.title }}
    </a>
  </h3>
  <p>{{ tutorial.description | markdownify }}</p>
{% endfor %}

