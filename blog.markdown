---
layout: page
title: Blog
permalink: /blog/
---
Welcome to my blog!

## SEO

<ul class="post-list">
  {% assign stories = site.data.seo | slice: 0, 3 %}
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

<button onclick="window.location.href='https://kjbritt.github.io/seo/';" style="background-color: #7f7053; color: white; padding: 15px 32px; border: none; border-radius: 8px; cursor: pointer; font-size: 16px;">More SEO stories</button>

## Wildlife

<ul class="post-list">
  {% assign stories = site.data.wildlife | slice: 0, 3 %}
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

<button onclick="window.location.href='https://kjbritt.github.io/wildlife/';" style="background-color: #7f7053; color: white; padding: 15px 32px; border: none; border-radius: 8px; cursor: pointer; font-size: 16px;">More Wildlife stories</button>