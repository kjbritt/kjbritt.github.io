---
layout: post
title:  "The pitfalls of using AI to write SEO meta descriptions"
author: "Keenan J. Britt"
description: "Writing quality meta descriptions for your web pages is a key feature of search engine optimization."
image: https://upload.wikimedia.org/wikipedia/commons/c/ce/Cartucho_de_Atari_2600_del_juego_Pitfall.jpg
date:   2026-01-11 08:06:33 +0000
category: seo
published: false
---
I'm a big advocate of automating efforts for search engine optimization (SEO) to save time and sanity. In a recent post, I explained the SEO importance of well-written meta descriptions and how you can [Automate your SEO efforts by scraping meta descriptions](https://kjbritt.github.io/seo/2026/01/04/automate-seo-meta-descriptions.html) with my Python script. 

However, some automation techniques should be approached with caution. I recently experimented with using AI large language models (LLMs) like Google Gemini to automatically generate optimized meta descriptions. Needless to say, the results were mixed. 
 

## Pitfall #1: AI hallucination

The first pitfall

## LLMs can't count

LLMs are infamously bad at counting, often failing to accurately count the number of words in a text or the number of letters in a word. LLMs don't process text character-by-character like traditional computer programs might, but rather in "tokens" which can be whole words or pieces of words. 

This common pitfall can mean that AI generated meta descriptions may be too long and end up being "truncated" (shortened) or ignored by search engines and replaced with something else in a search results page. To avoid being truncated, meta descriptions should ideally be no longer than 160 characters. 

I provided Google Gemini with the title of this blog post ("The pitfalls of using AI to write SEO meta descriptions") and asked it to return an ideal meta description between 150 and 160 characters in length. Gemini instantly returned a blurb:

>__Description__: Can AI ruin your rankings? Discover the risks of using AI for meta descriptions, from robotic phrasing to "hallucinated" facts. Learn how to keep your SEO human-centric for better CTR. (160 characters)

Gemini was quite confident that the description it provided was only 160 characters. Gemini later told me that it is "exactly 160 characters, hitting the maximum limit for a desktop snippet while remaining concise enough for mobile."

The problem is that the text Gemini provided is actually 184 characters. I then asked Gemini to provide meta descriptions for web pages from a series of local businesses. I found that Gemini persistently exceeded the recommended character count, sometimes producing descriptions in excess of 200 characters. 

If you're ever worried about AI stealing your job, remember that you still advantage over the current major LLMs if you happen to know how to count. 

## You may be wasting your time

text

As Google explained in the article [“Control your snippet in search results”](https://developers.google.com/search/docs/appearance/snippet):

>Google will sometimes use the <meta name="description"> tag from a page to generate a snippet in search results, if we think it gives users a more accurate description than would be possible purely from the on-page content. A meta description tag generally informs and interests users with a short, relevant summary of what a particular page is about. They are like a pitch that convince the user that the page is exactly what they’re looking for.