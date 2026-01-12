---
layout: post
title:  "The pitfalls of using AI to write SEO meta descriptions"
author: "Keenan J. Britt"
description: "Are you using AI to automate your SEO efforts? Beware these three common pitfalls if you're using LLMs to write meta descriptions for your web pages."
image: https://upload.wikimedia.org/wikipedia/commons/c/ce/Cartucho_de_Atari_2600_del_juego_Pitfall.jpg
date:   2026-01-11 08:06:33 +0000
category: seo
published: true
---
I'm a big advocate of automating efforts for search engine optimization (SEO) to save time and sanity. In a recent post, I explained the SEO importance of well-written meta descriptions and how you can [Automate your SEO efforts by scraping meta descriptions](https://kjbritt.github.io/seo/2026/01/04/automate-seo-meta-descriptions.html) with my Python script. 

However, some automation techniques should be approached with caution. I recently experimented with using AI large language models (LLMs) like Google Gemini to automatically generate optimized meta descriptions. Needless to say, the results were mixed. 
 

## Pitfall #1: AI hallucination

The first pitfall is one you might guess: [hallucination](https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)). Within AI, "hallucination" refers to the habit of LLMs and other AI tools to fabricate details that are inaccurate. LLMs are notorious for not just hallucinating, but confidently asserting that their hallucinations are correct.

If you're using an LLM to write meta descriptions for your web pages, you will need to carefully edit and fact-check the descriptions it provides. I experimented with this by providing Google Gemini with the URLs to websites from a number of local businesses and asked it to provide optimized meta descriptions that would drive click-through-rate. I found that Gemini would often hallucinate and keyword-stuff the descriptions with services that weren't actually provided by those businesses.

For example, I gave Gemini the link to the homepage of the [Musk Ox Farm](https://www.muskoxfarm.org/). It provided this as a suggested meta description:

>Visit our historic farm for a close-up look at the majestic musk ox. Take a guided tour, learn about Ice Age history, and shop for rare, hand-combed qiviut fiber.

Gemini correctly indicated that the Musk Ox Farm offers guided tours and a qiviut gift shop, but it hallucinated the details about the tours invovling "Ice Age history". Although musk oxen are sometimes described as "Ice Age survivors", the term "Ice Age" does not even appear on the Farm's homepage.

## Pitfall #2: LLMs can't count

LLMs are infamously bad at counting, often failing to accurately count the number of words in a text or the number of letters in a word. LLMs don't process text character-by-character like traditional computer programs might, but rather in "tokens" which can be whole words or pieces of words. 

This common pitfall can mean that AI generated meta descriptions may be too long and end up being "truncated" (shortened) or ignored by search engines and replaced with something else in a search results page. To avoid being truncated, meta descriptions should ideally be no longer than 160 characters. 

I provided Google Gemini with the title of this blog post ("The pitfalls of using AI to write SEO meta descriptions") and asked it to return an ideal meta description between 150 and 160 characters in length. Gemini instantly returned a blurb:

>__Description__: Can AI ruin your rankings? Discover the risks of using AI for meta descriptions, from robotic phrasing to "hallucinated" facts. Learn how to keep your SEO human-centric for better CTR. (160 characters)

Gemini was quite confident that the description it provided was only 160 characters. Gemini later told me that it is "exactly 160 characters, hitting the maximum limit for a desktop snippet while remaining concise enough for mobile."

The problem is that the text Gemini provided is actually 184 characters. I then asked Gemini to provide meta descriptions for web pages from a series of local businesses. I found that Gemini persistently exceeded the recommended character count, sometimes producing descriptions in excess of 200 characters. 

If you're ever worried about AI stealing your job, remember that you still advantage over the current major LLMs if you happen to know how to count. 

## Pitfall #3: You may be wasting your time

No matter how well-written your meta descriptions are, there's no guarantee that search engines will display them in a search results page. Search engines often ignore meta descriptions to create their own snippets. As Google explained in the article [“Control your snippet in search results”](https://developers.google.com/search/docs/appearance/snippet):

>Snippets are automatically created from page content. Snippets are designed to emphasize and preview the page content that best relates to a user's specific search. This means that Google Search might show different snippets for different searches. Snippets are primarily created from the page content itself. However, Google sometimes uses the meta description HTML element if it might give users a more accurate description of the page than content taken directly from the page.

You'll still want to optimize your meta descriptions for the important pages on your website, but it may not be worth your time to write something special for each page on a large website, especially if many of those pages don't contain content you're trying to rank for as part of your SEO strategy. 

Having an LLM analyze those less important pages to produce meta descriptions that you have to then fact-check, edit and shorten would become a significant time burden. If a particular web page isn't part of your SEO strategy, feel free to let the search engines write their own snippets and focus your time on more productive SEO efforts. 