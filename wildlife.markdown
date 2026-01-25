---
layout: page
title: Wildlife
permalink: /wildlife/
---
Welcome to my wildlife blog! From wolves to whales, moose to musk oxen, I've been honored to have (safe) encounters with many of Alaska's iconic wildlife species. 

## Recent posts

<ul class="post-list">
  {% assign stories = site.data.wildlife | slice: 0, 5 %}
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

<details>
  <summary>Older posts</summary>
<ul class="post-list">
  {% assign stories = site.data.wildlife | slice: 5, 10 %}
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
</details>