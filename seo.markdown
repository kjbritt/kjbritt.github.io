---
layout: page
title: SEO
permalink: seo/
tag: seo
---
<figure>
  <img src="/docs/assets/images/vegas_strip.jpg" alt="A view of the Las Vegas strip at night with the Bellagio fountains" />
  <figcaption><i>The Vegas Strip, Las Vegas, Nevada, October 2021</i></figcaption>
</figure>


Welcome to my new SEO blog!

## Recent posts

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