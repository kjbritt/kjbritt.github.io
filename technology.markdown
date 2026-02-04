---
layout: page
title: Technology
permalink: /technology/
image: /docs/assets/images/radio.jpg
---
<figure>
  <img src="/docs/assets/images/radio.jpg" alt="A portable AM/FM radio on the balcony of a cruise ship cabin" />
  <figcaption><i>An AM/FM radio tuned into Cuban radio, Caribbean Sea, November 2022</i></figcaption>
</figure>

Welcome to my new technology blog!

## Recent posts

<ul class="post-list">
  {% assign stories = site.data.technology | slice: 0, 5 %}
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