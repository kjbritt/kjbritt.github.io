---
layout: post
title:  "Automate your SEO efforts by scraping meta descriptions"
author: "Keenan J. Britt"
description: "Writing quality meta descriptions for your web pages is a key feature of search engine optimization."
image: https://upload.wikimedia.org/wikipedia/commons/thumb/e/ef/Programming_code.jpg/960px-Programming_code.jpg
date:   2026-01-04 01:06:33 +0000
category: seo
tag: seo
published: true
---
{% include breadcrumbs.html %}

Writing quality meta descriptions for your web pages is a key feature of search engine optimization (SEO). 

## What are meta descriptions?

Meta descriptions are short "blurbs" or "snippets" describing the content of your web page. Ideally, these descriptions should be about 150 to 160 charactes in length. Though not guranteed, search engines like Google may display a web page's meta description on a search engine results page (SERP).

As Google explained in the article "[Control your snippet in search results](https://developers.google.com/search/docs/appearance/snippet)":

>Google will sometimes use the `<meta name="description">` tag from a page to generate a snippet in search results, if we think it gives users a more accurate description than would be possible purely from the on-page content. A meta description tag generally informs and interests users with a short, relevant summary of what a particular page is about. They are like a pitch that convince the user that the page is exactly what they're looking for.

You can easily find a web page's meta description (if it has one) by viewing the page's source code. If you're using a modern browser like Chrome or Firefox on a PC, you can hit Ctrl + U (or right-click and select "View Page Source") while visiting the web page. The HTML code for the meta description will look something like this: `<meta name="description" content="Gallia est omnis divisia in partes tres.">`. Can you find the meta description for this post?

## Why are meta descriptions important for SEO?

Meta descriptions are not considered to be a ranking factor in search engine algorithms like titles, headings and page content. However, well-written meta descriptions can still improve your SEO and drive visitors to your web page. The meta description is your "pitch" to your potential customers as they scroll through the SERP. 

As [Yoast explains](https://yoast.com/meta-descriptions/):

>Google uses click-through rate (CTR) to determine whether you’re a good result. If more people click on your result, Google considers you to be a good result and will, based on your position, move you up the rankings. 

SEO efforts should always, ultimately, be aimed at humans, not bots. You'll want to periodically review your web pages' meta descriptions to ensure they are accurate and up-to-date. Overtime, meta descriptions may become dated, containing references to products or services your organization no longer offers. They may also use old branding language that no longer reflects your brand identity. As you edit or rewrite your meta descriptions, make sure to follow Google's guidelines on "[best practices for creating quality meta descriptions](https://developers.google.com/search/docs/appearance/snippet#meta-descriptions)".

## How to automatically pull meta descriptions from every page on your website

If you've taken over management of a website with a significant number of pages, navigating through a content management system (CMS) to manually review the meta description for each page can take a significant amount of time. 

Thankfully, there's a quick solution to easily pull a complete list of all the meta descriptions across your website as a spreadsheet to quickly and easily identify those that need to be updated.

You can scrape all the meta descriptions from your website using my new [Meta Description Scraper](https://github.com/kjbritt/Meta-Description-Scraper). Using this scraper will automate your SEO efforts and save valuable time.

You will need to have Python installed on your machine for the program to work. If you don't have Python installed, you can easily [download the latest version](https://www.python.org/downloads/) for free. After that, you can download my Meta Description Scraper from my GitHub repositories and run it from your computer's command line (Command Prompt on Windows) to receive a CSV file in seconds. 

The script will prompt you to enter the name of a TXT file containing all the URLs from your website. Make sure the file you intend to use is saved in the same folder as the Python script. You can easily extract a list of all web page URLs contained in your website's sitemap using the [SEOwl Sitemap Extractor](https://www.seowl.co/sitemap-extractor/). 

After iterating through each of the URLs in the TXT file, the script will produce a report titled meta_descriptions.csv for you to review. 



_The meta image used on this webpage is courtesy of Martin Vorel, under a Creative Commons ASA 4.0 license, [via Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Programming_code.jpg)._