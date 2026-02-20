---
layout: post
title:  "Can AI save Florida's coral reef? These scientists think so"
author: "Keenan J. Britt"
description: "These scientists believe AI can help forecast coral bleaching weeks in advance, giving human reef managers time to prepare."
image: /docs/assets/images/Florida_Reef.jpg
date:   2026-02-17 01:06:33 +0000
category: technology
tags: technology marinebio
published: true
---
{% include breadcrumbs.html %}
<figure>
  <img src="/docs/assets/images/Florida_Reef.jpg" alt="A coral reef in Florida." />
  <figcaption><i>Elkhorn coral on Molasses Reef, Florida. Photo by Jim Stuby and in the Public Domain, <a href="https://en.wikipedia.org/wiki/Florida_Reef#/media/File:Elkhorn_coral_8_Molasses_Reef_20080309.jpg">via Wikimedia Commons</a>.</i></figcaption>
</figure>

Located along the seaward side of the Florida Keys, the [Florida Reef](https://en.wikipedia.org/wiki/Florida_Reef) is the only living barrier reef in the Lower 48. The Florida Reef is composed of over 6,000 smaller, individual reefs, and is home to hundreds of species of marine vertebrates and dozens of species of coral. 

Sadly, the Florida Reef, like many reefs around the world, is threatened by rising ocean temperatures due to climate change. Warmer water temperatures may result in <a href="https://oceanservice.noaa.gov/facts/coral_bleach.html"><dfn>coral bleaching</dfn></a> in which corals expel the algae living in their tissues, leaving the coral white in color. The bleached coral is still alive, but much more likely to die due to disease, starvation or stress. 

Coral bleaching has been a major threat to America's coral reefs. According to the National Oceanic and Atmospheric Administration (NOAA), in 2005 the U.S. "lost half of its coral reefs in the Caribbean in one year due to a massive bleaching event [...] centered around the northern Antilles near the Virgin Islands and Puerto Rico."

What can be done to help protect the Florida Reef from future coral bleaching events? A team of environmental and data scientists believe AI might be able to help forecast coral heat stress weeks in advance, giving human reef managers time to prepare. 

In a paper published in December, titled <cite><a href="https://iopscience.iop.org/article/10.1088/2515-7620/ae2570">An explainable machine learning prediction system for early warning of heat stress on Florida’s Coral Reef</a></cite>, the team introduced a machine-learning framework that they argued is capable of "forecasting the onset of moderate coral heat stress at site specific resolution" along the Florida Reef. 

[Marybeth Carmela Arcodia](https://people.miami.edu/profile/5fc103221a3deb9dce777c4cfafa9523), Ph.D., an assistant professor at the University of Miami, was the lead author on the paper, joined by co-authors [Richard Karp](https://coralreeffutures.earth.miami.edu/people/lab-alumni/rich-karp/index.html), Ph.D., also with the University of Miami, and [Elizabeth A. Barnes](https://www.bu.edu/cds-faculty/profile/elizabeth-a-barnes/), Ph.D., with Boston University. 

The team trained their machine learning model on a 40 year data set, spanning 1985 to 2024, available online from NOAA's [Coral Reef Watch](https://coralreefwatch.noaa.gov/) website, covering ocean temperatures at specific locations in the Florida Reef. For the study, the authors had the model focus on three specific parts of the Florida Reef system: Sand Key, Sombrero Reef and Molasses Reef. The model uses a Python version of the [XGBoost](https://en.wikipedia.org/wiki/XGBoost) algorithm.

After training and testing their model, the team found that the model can predict coral heat stress "up to six weeks in advance, with an average error of about one week," outperforming traditional forecasting models. Having an early warning system for when coral reefs will be in danger could provide a key tool for future conservation efforts. The authors explained in the paper that:

>"This tool offers insight for managers with information to focus monitoring and response efforts where and when they are needed most. These early warnings can be used to trigger emergency actions, such as increasing monitoring or deploying intervention and supporting more proactive and locally tailored reef conservation."

The code used in the project is publicly available on [Arcodia's GitHub repository](https://github.com/mbarcodia/coral_stress_prediction_xgb/tree/main). 