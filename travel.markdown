---
layout: page
title: Travel
permalink: /travel/
image: /docs/assets/images/coba.jpg
---
<figure>
  <img src="/docs/assets/images/coba.jpg" alt="A Mayan pyramid at Coba,Mexico" />
  <figcaption><em>A Mayan pyramid at Coba, Quintana Roo, Mexico. November 2022.</em></figcaption>
</figure>


Welcome to my new travel blog.

## Recent posts

<ul>
{% for post in site.tags[page.tag] %}
  <li>
    {{ post.date | date: "%B %d, %Y" }}: <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>