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

<ul>
  {% assign stories = site.data.news | slice: 0, 5 %}
  {% for story in stories %}
    <li>
      <a href="{{ story.url }}">{{ story.title }}</a>
    </li>
  {% endfor %}
</ul>