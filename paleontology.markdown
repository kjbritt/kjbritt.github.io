---
layout: page
title: Paleontology
permalink: /paleontology/
image: /docs/assets/images/allosaurus.jpg
---

![An Allosaurus dinosaur skeleton at a museum](/docs/assets/images/allosaurus.jpg)
_An Allosaurus on display at the University of Michigan, January 2012_

Welcome to my new paleontology blog! 

## Recent posts

<ul class="post-list">
  {% assign stories = site.data.paleontology | slice: 0, 5 %}
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
  {% assign stories = site.data.paleontology | slice: 5, 10 %}
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