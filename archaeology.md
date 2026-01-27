---
layout: page
title: Archaeology
permalink: /archaeology/
---
I hold a bachelor's degree in anthropology from the University of Michigan. While I was trained in four-field anthropology, my area of focus was in archaeology. 

## Field Work

- Maya Research Program, Blue Creek, Belize, 2012
- Khirbet Iskander Expedition, Madaba, Jordan, 2013
- Field School in Athabaskan Prehistory, Delta Junction, Alaska, 2016

## News

Latest news.

<ul class="post-list">
  {% assign stories = site.data.news | slice: 0, 5 %}
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