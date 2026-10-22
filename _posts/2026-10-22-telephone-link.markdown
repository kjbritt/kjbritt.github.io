---
layout: post
title:  "How to add and style telephone links on your web pages"
author: "Keenan J. Britt"
description: "Who ya gonna call?"
image: /docs/assets/images/WebDesign_meta.jpg
date:   2026-10-21 01:06:33 +0000
category: webdesign
tags: webdesign
published: true
---
{% include breadcrumbs.html %}

Adding a telephone link can be a simple addition to your website's contact page. Usually, website CMS platforms will automatically hyperlink an email address without you having to manually add in the "mailto" link, but that generally isn't the case with phone numbers.

It's super convienent for mobile users visiting your website if they can simply click the telephone link and have their phone dial that number automatically. But how do you properly hyperlink this?

In order to hyperlink a phone number in HTML, you'll need to use a telephone link inside your anchor tag's href attribute. The format will need to be <code>"tel:+15551234567"</code> if your number is something like "(555) 123-4567". That being said, you can still style the link text to which ever format you prefer. 

You can try this out and look at sample code in the W3Schools' [online HTML editor](https://www.w3schools.com/tags/tryit.asp?filename=tryhtml_link_phoneto). 

Here's an example of how you might implement this along with an email address on a contact page:

<div style="background-color: #D3D3D3; padding: 10px; color:black;">
  <h3>Contact</h3>
<ul>
<li>Special Agent Fox Mulder</li>
<li><a href="mailto:spooky@fbi.gov">spooky@fbi.gov</a></li>
<li><a href="tel:+12025553574">(202) 555-3574</a></li>
</ul>
</div>

## Getting more creative

You can also get more creative by adding a button your web visitors can click on. The buton text can serve as a nice place to add a call to action like "Call Now!" or something similar. You can add the telephone link into the JavaScript onclick attribute as <code>"location.href='tel:+15551234567'</code>. For fun, you could try adding a graphic like the [Font Awesome telephone receiver icon](https://www.w3schools.com/icons/tryit.asp?filename=tryicons_fa-phone). 

Here's an example for a ghost busting service:

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<button style="font-size:24px" onclick="location.href='tel:+12125552368';"><i class="fa fa-phone"></i> Who ya gonna call?</button>

## Related news

- [Web accessibility: are you using proper bulleted lists?](https://kjbritt.github.io/webdesign/2026/03/21/bulleted-lists.html)


