---
layout: page
title: Paleontology
permalink: /paleontology/
image: /docs/assets/images/allosaurus.jpg
---
<figure>
  <img src="/docs/assets/images/allosaurus.jpg" alt="An Allosaurus dinosaur skeleton at a museum" />
  <figcaption><em>An Allosaurus on display at the University of Michigan, January 2012</em></figcaption>
</figure>


Welcome to my new paleontology blog! I'm a lifelong paleo-fan. If you would like to submit a news tip, collaborate on something, or just have a bone-to-pick, feel free to [Contact](/contact) me. 

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