---
layout: post
title:  "Automate your SEO by finding broken links with Python"
author: "Keenan J. Britt"
description: "Are you using AI to automate your SEO efforts? Beware these three common pitfalls if you're using LLMs to write meta descriptions for your web pages."
image: https://upload.wikimedia.org/wikipedia/commons/a/a3/404_Not_Found.jpg
date:   2026-01-17 08:06:33 +0000
category: seo
published: true
---
Early in my career as a web manager, I was often tasked with searching over websites manually checking for "broken links" (on-page hyperlinks that lead to interal or external 404 pages). As I sat scrolling, clicking, scrolling and clicking through web pages making sure each of the links worked, I often thought to myself "surely there's a more efficient way to do this?". 

Thankfully, I was also "learning to code" in Python at the time. I soon discovered that the Python programming language offers plenty of libraries that can help automate tasks like checking for broken 404 links on a website. 

With a few simple Python scripts that you can run from your own computer, you to can easily automate the hunt for broken links on the websites that you manage. 

## Are 404 links bad for SEO?

There's been some confusion on the internet about whether or not 404 errors are actually bad for SEO. If a user enters an incorrect URL into their browser to a page that doesn't actually exist (something like [https://kjbritt.github.io/doesNotExist](https://kjbritt.github.io/)), you'll want a 404 error landing page to appear to help them find what they're looking for. 

However, 404 errors can be bad for your SEO if they are a result of broken links existing on your web pages. As [Adrian Cojocariu](https://cognitiveseo.com/blog/author/coadr93/) explained on [CognitiveSEO](https://cognitiveseo.com/blog/19933/do-404-errors-affect-seo/): 

>The only type of 404 links that really hurt your website are the ones that are on it. When you add a link from your website to another website, you have to make sure that URL actually exists or that you don’t misspell it. You might also have internal links that are broken...Broken links create bad user experience and we all know that Google (and probably other search engines as well) cares about user experience.

## Find all broken links across your site

Thankfully, there are easy automation tools that can allow you to quickly identify all broken links across your website. 

If you have [Python installed on your machine](https://www.python.org/downloads/), you can try my [404-Broken-Link-Finder](https://github.com/kjbritt/404-Broken-Link-Finder). In addition to Python, you will also need to install Python's [BeautifulSoup](https://beautiful-soup-4.readthedocs.io/en/latest/#) library. 

My 404-Broken-Link-Finder is a simple script that you can run from the command line on your machine. It will ask you to provide a TXT file containing the web page URLs you want to scan and then check each and every https/http link on each and every one of the provided URLs. Any links that return a 404 status code will be included on a CSV spreadsheet titled 'link_status_codes.csv' that you can view after the program finishes running.

## Related Posts

- [The pitfalls of using AI to write SEO meta descriptions](https://kjbritt.github.io/seo/2026/01/11/pitfalls-ai-meta-descriptions.html)
- [Automate your SEO efforts by scraping meta descriptions](https://kjbritt.github.io/seo/2026/01/04/automate-seo-meta-descriptions.html)

_The meta image used on this webpage is courtesy of Yorqulov Husan, under a Creative Commons Attribution 4.0 International license, [via Wikimedia Commons](https://commons.wikimedia.org/wiki/File:404_Not_Found.jpg)._