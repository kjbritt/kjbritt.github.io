---
layout: page
title: Philosophy
permalink: /philosophy/
tag: philosophy
---


Welcome to my new philosophy blog!

## Recent posts

<ul>
{% for post in site.tags[page.tag] %}
  <li>
    {{ post.date | date: "%B %d, %Y" }}: <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>