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

You don't have to write out HTML code to create a proper bulleted list. Most likely, if you're using a CMS, they'll be a button to do this through your WYSIWYG editor.

## Avoid using emoji lists

A popular trend inspired by social media is to use emojis to create lists using emojis as bullets. It's even possible to create proper HTML bulleted lists with emojis as the bullets. The Mozilla Developers Network [provides this example](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/list-style-type) by styling the CSS list-style-type property.

I can use the list-style-type property to style my list with the sauropod emoji and it does come across _looking_ professional.

<ul style="list-style-type: '\1F995';">
  <li>Diplodocus</li>
  <li>Barosaurus</li>
  <li>Camarasaurus</li>
  <li>Brachiosaurus</li>
</ul> 

However, this can be really annoying to listen to on a screen reader, since assistive technology often reads emojis out loud to users. Narrator read this list to me as "sauropod Diplodocus, sauropod Barosaurus, sauropod Camarasaurus, sauropod Brachiosaurs."

Emojis can be used in designs, but they should be used sparingly. Accessibility blogger Life of a Blind Girl [explained in a post](https://lifeofablindgirl.com/2023/04/02/your-a-z-guide-for-social-media-accessibility/):

>It’s ok to use emojis, just don’t overuse them. Screen readers read out a description for every single one. Having multiple emojis read out loud is a frustrating, tedious experience for screen reader users. In some cases, it doubles the time it takes to read a post when having to listen to a mass of emojis being read out loud.


## What if you want fancy bullets?

Accessible web design doesn't mean _boring_ web design. It's possible to design features that are interesting _and_ accessible for all users. While you may need to work with a developer, it is possible to created bulleted lists that display emojis for sighted users but remove the emojis for assistive technology. 

For those interested in accessible bulleted lists, web designer Chris Coyier provides some helpful CSS code in his blog post [Emoji Lists, The Good Way?](https://chriscoyier.net/2023/04/07/emoji-lists-the-good-way/).

## What about social media posts?

Someone asked me once about how to create accessible bulleted lists on social media posts, and I honestly don't have an answer. Most major social media platforms like Facebook, Instagram, X and Bluesky do not have WYSIWYG editors with buttons for bulleted lists or options to add HTML. Google's AI overview suggested the simplest way was to do this is to "use standard bullet characters (like •) followed by a space, rather than emojis or dashes, to ensure screen readers interpret them correctly."

I tried this out on my Bluesky and found that Narrator read the names of the dinosaurs without reading the name of the bullet character. 

<blockquote class="bluesky-embed" data-bluesky-uri="at://did:plc:jpxscn2y2q4iy5agzxy4bry7/app.bsky.feed.post/3mhn5sczft223" data-bluesky-cid="bafyreigmnwk4ben2ksfa6cuhhsr3dhyd3k4klzqihxcebn4xfpzuroduh4" data-bluesky-embed-color-mode="system"><p lang="en">Just some of my favorite sauropods:

•Diplodocus
•Barosaurus
•Camarasaurus
•Brachiosaurus</p>&mdash; Digging Deeper with K.J. Britt (<a href="https://bsky.app/profile/did:plc:jpxscn2y2q4iy5agzxy4bry7?ref_src=embed">@kjbritt.bsky.social</a>) <a href="https://bsky.app/profile/did:plc:jpxscn2y2q4iy5agzxy4bry7/post/3mhn5sczft223?ref_src=embed">March 22, 2026 at 12:45 AM</a></blockquote><script async src="https://embed.bsky.app/static/embed.js" charset="utf-8"></script>

If anyone else knows a better way to make accessible bulleted lists on social media, please [Contact me](https://kjbritt.github.io/contact/). 

## Digging deeper

If you'd like to start digging deeper into this topic, Princeton University's Digital Accessibility Program has [a helpful article with more details](https://digital.accessibility.princeton.edu/how/content/lists).

