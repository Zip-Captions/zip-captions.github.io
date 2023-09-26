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

Search our [help documentation]({{ site.baseurl }}{% link help.md %})

Search our [knowledge base]({{ site.baseurl }}{% link kb.md %})

<hr>
<h2>Most Recent Updates</h2>
<ul class="entries">
   {% for post in site.posts limit:2 %}
    <h2>
      <a href="{{ post.url | prepend: site.baseurl}}">
        {{ post.title }}
      </a>
    </h2>
{% endfor %}
</ul>


