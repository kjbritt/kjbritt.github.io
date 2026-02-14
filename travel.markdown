---
layout: page
title: Travel
permalink: /travel/
image: /docs/assets/images/coba.jpg
tag: travel
---
<figure>
  <img src="/docs/assets/images/coba.jpg" alt="A Mayan pyramid at Coba,Mexico" />
  <figcaption><em>A Mayan pyramid at Coba, Quintana Roo, Mexico. November 2022.</em></figcaption>
</figure>


Welcome to my new travel blog.

## Recent posts

<ul class="post-list">
  {% assign stories = site.tags[page.tag] | slice: 0, 5 %}
  {% for story in stories %}
    <li style="margin-bottom: 20px;">
      <span class="post-meta">{{ story.date | date: "%B %e, %Y" }}</span>
      <h3>
        <a class="post-link" href="{{ story.url }}">
          {{ story.title }}
        </a>
      </h3>
    </li>
  {% endfor %}
</ul>