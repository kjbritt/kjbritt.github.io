---
layout: page
title: Archaeology
permalink: /archaeology/
image: /docs/assets/images/petra_pfp.jpg
---
<figure>
  <img src="/docs/assets/images/petra_pfp.jpg" alt="A college student on a donkey at Petra, Jordan" />
  <figcaption><em>A naive, young student of archaeology at Petra, Jordan, June 2013</em></figcaption>
</figure>

I hold a bachelor's degree in anthropology from the University of Michigan. While I was trained in four-field anthropology, my area of focus was in archaeology. I have participated in archaeological digs in Belize, Jordan and Alaska. 

## Latest posts

<ul class="post-list">
  {% assign stories = site.data.archaeology | slice: 0, 5 %}
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