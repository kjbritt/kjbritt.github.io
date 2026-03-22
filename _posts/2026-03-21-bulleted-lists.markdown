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

However, these improper bulleted lists can cause serious accessibility issues for some of your web visitors, including those who are blind or visually impaired and using a screen reader. 

## Creating an unordered list

Here's a simple list of sauropod ("long neck") dinosaurs known from the Jurassic Period of the Western United States. This list is in a proper HTML bulleted list.

<ul>
  <li>Diplodocus</li>
  <li>Barosaurus</li>
  <li>Camarasaurus</li>
  <li>Brachiosaurus</li>
</ul>

And here's a list I made just using some asterisks:

*Diplodocus<br>
*Barosaurus<br>
*Camarasaurus<br>
*Brachiosaurus<br>

See the difference? Your sighted users will likely notice that the second list looks less professional than the proper bullets. Web visitors using screen readers will be able to _hear_ the difference. Their screen reader will likely announce to them that the first list is a bulleted list and then read the bullets, while the second list will be read as "asterisk Diplodocus, asterisk Barosaurus, asterisk Camarasaurus, asterisk Brachiosaurus."

You can even try this out for yourself. Your computer likely has a screen reader available, pre-installed. I use Narrator, which comes with Windows 11. 

## Avoid using emoji lists

A popular trend inspired by social media is to use emojis to create lists using emojis as bullets. It's even possible to create proper HTML bulleted lists with emojis as the bullets. The Mozilla Developers Network [even provides this example](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/list-style-type) by styling the CSS list-style-type property:

<ul style="list-style-type: space-counter;">
  <li>Apollo</li>
  <li>Hubble</li>
  <li>Chandra</li>
  <li>Cassini-Huygens</li>
</ul> 

Accessibility blogger Life of a Blind Girl [explained in a post](https://lifeofablindgirl.com/2023/04/02/your-a-z-guide-for-social-media-accessibility/):

>It’s ok to use emojis, just don’t overuse them. Screen readers read out a description for every single one. Having multiple emojis read out loud is a frustrating, tedious experience for screen reader users. In some cases, it doubles the time it takes to read a post when having to listen to a mass of emojis being read out loud.



<ul style="list-style-type: '\1F995';">
  <li>Diplodocus</li>
  <li>Barosaurus</li>
  <li>Camarasaurus</li>
  <li>Brachiosaurus</li>
</ul> 


## What if you want fancy bullets?

Accessible web design doesn't mean _boring_ web design. It's possible to design features that are interesting _and_ accessible for all users. While you may need to work with a developer, it is possible to created bulleted lists that display emojis for sighted users but remove the emojis for assistive technology. 

For those interested in accessible bulleted lists, web designer Chris Coyier provides some helpful CSS code in his blog post [Emoji Lists, The Good Way?](https://chriscoyier.net/2023/04/07/emoji-lists-the-good-way/).

