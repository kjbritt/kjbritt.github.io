---
layout: page
title: Marine Biology
permalink: marinebio/
tag: marinebio
---
<figure>
  <img src="/docs/assets/images/oregon_spacex.jpg" alt="SpaceX Falcon 9 rocket burning up over Hillsboro, Oregon." />
  <figcaption><em>SpaceX Falcon 9 rocket burning up over Hillsboro, Oregon. March 2021.</em></figcaption>
</figure>

Welcome to my new marine biology blog!

## Recent news

<ul class="post-list">
  {% assign stories = site.tags[page.tag] | slice: 0, 5 %}
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