---
layout: post
title:  "Web accessibility: are you using proper bulleted lists?"
author: "Keenan J. Britt"
description: "Web accessibility: are you using proper bulleted lists?"
image: /docs/assets/images/WebDesign_meta.jpg
date:   2026-03-21 01:06:33 +0000
category: webdesign
tags: webdesign accessibility
published: true
---
{% include breadcrumbs.html %}

A common web accessibility mistake is to use improper bulleted lists on a web page or in an email. This often happens accidently, if someone copy-pastes a list from a text document or is unaware of proper bulleting in HTML. Sometimes folks will simply use asterisks or dashes instead of bullet points; other times, web editors may use emojis to create trendy-looking bullet points.

However, these improper bulleted lists can cause serious accessibility issues for some of your web visitors, inclulding those who are blind or visually impaired and using a screen reader. 

## Creating an ordered list

Here's a simple list of sauropod ("long neck") dinosaurs known from the Jurassic Period of the Western United States. This list is in a proper HTML bulleted list.

<ul>
  <li>Diplodocus</li>
  <li>Barosaurus</li>
  <li>Camarasaurus</li>
  <li>Brachiosaurus</li>
</ul>

And here's a list I made just using some asterisks:

*Diplodocus
*Barosaurus
*Camarasaurus
*Brachiosaurus

See the difference?

## What if you want fancy bullets?

<ul style="list-style-type:circle;">
  <li>Diplodocus</li>
  <li>Barosaurus</li>
  <li>Camarasaurus</li>
  <li>Brachiosaurus</li>
</ul>

