---
layout: page
title: Paleontology
permalink: /paleontology/
image: /docs/assets/images/allosaurus.jpg
---

![An adult female musk ox named Eider](/docs/assets/images/allosaurus.jpg)
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