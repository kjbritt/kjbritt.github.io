---
layout: page
title: Technology
permalink: technology/
image: /docs/assets/images/Technology_meta.jpg
tag: technology
---
<figure>
  <img src="/docs/assets/images/radio.jpg" alt="A portable AM/FM radio on the balcony of a cruise ship cabin" />
  <figcaption><i>An AM/FM radio tuned into Cuban radio, Caribbean Sea, November 2022</i></figcaption>
</figure>

Welcome to my new technology blog!

## Recent news

{% include recentposts.html %}
 

## Older news

<details>
  <summary onclick="this.innerText = this.parentElement.open ? 'Display older news' : 'Hide older news'"
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
    transition: background 0.3s ease;">Display older news</summary>
<ul class="post-list">
  {% assign stories = site.tags[page.tag] | slice: 5, 10 %}
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