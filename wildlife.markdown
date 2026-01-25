---
layout: page
title: Wildlife
permalink: /wildlife/
description: "Welcome to my wildlife blog! From wolves to whales, moose to musk oxen, I've been honored to have had encounters with many of Alaska's iconic wildlife species."
image: /docs/assets/images/eider_web.jpg
---
![An adult female musk ox named Eider](/docs/assets/images/eider_web.jpg)
_Eider, the world's prettiest musk ox, March 2025_

Welcome to my wildlife blog! From wolves to whales, moose to musk oxen, I've been honored to have had encounters with many of Alaska's iconic wildlife species. 

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

## Older posts

<details>
  <summary onclick="this.innerText = this.parentElement.open ? 'Display older posts' : 'Hide older posts'"
  style="
    display: inline-block;
    padding: 10px 20px;
    background-color: #7f7053;
    color: white;
    border-radius: 5px;
    cursor: pointer;
    font-family: sans-serif;
    font-weight: bold;
    list-style: none;
    user-select: none;
    transition: background 0.3s ease;">Display older posts</summary>
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