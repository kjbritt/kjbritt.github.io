---
layout: page
title: SEO
permalink: /seo/
---
Welcome to my new SEO blog!

## Recent posts

<ul class="post-list">
  {% assign stories = site.data.seo | slice: 0, 5 %}
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