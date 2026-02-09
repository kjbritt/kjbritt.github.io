---
layout: post
title:  "How to visit the Montana Dinosaur Center this summer"
author: "Keenan J. Britt"
description: "You can visit this scenic dinosaur attraction this summer."
image: /docs/assets/images/carpenter_site_views.jpg
date:   2026-02-08 01:06:33 +0000
category: travel
tag: travel
published: true
---
{% include breadcrumbs.html %}

You can visit the [Montana Dinosaur Center](https://tmdinosaurcenter.org/) in Bynum, Montana this summer. The center is located along along US Highway 89, making it an easy stop for travelers jumping from  Yellowstone to Glacier National Park.

## Summer 2026 planning

<iframe src="https://www.facebook.com/plugins/post.php?href=https%3A%2F%2Fwww.facebook.com%2Ftmdinosaurcenter%2Fposts%2Fpfbid06rbPLTGRYUPw2TsCs1mMv4SXXubDmeQwFNUoCY7xLpnPeyZ7gzPBiav2igjSsLjEl&show_text=true&width=500" width="500" height="572" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe><br>

The Montana Dinosaur Center advises visitors to check "the Glacier National Park website for the latest updates as you map out your route". Alerts are available online from [the park's website](https://www.nps.gov/glac/index.htm). You can also view park status updates below which are available here via the [National Park Service API](https://www.nps.gov/subjects/developer/api-documentation.htm#/alerts/getAlerts). 

<style>
        
        #alert-container { max-width: 800px; margin: auto; }
        .alert-card {
            background: white;
            padding: 15px;
            margin-bottom: 15px;
            border-left: 10px solid #ccc;
            border-radius: 4px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        /* Color coding by category */
        .danger { border-left-color: #d9534f; } /* Red */
        .closure { border-left-color: #333; }    /* Black */
        .caution { border-left-color: #f0ad4e; } /* Orange */
        .info { border-left-color: #5bc0de; }    /* Blue */

        h2 { margin-top: 0; font-size: 1.2rem; }
        .category-badge {
            text-transform: uppercase;
            font-size: 0.7rem;
            font-weight: bold;
            display: block;
            color: #666;
        }
    </style>


<div id="alert-container">
        <h2>Glacier National Park Status</h2>
        <p>Loading current alerts...</p>
        </div>

<script>
        const apiKey = 'iwHREkxKsMlL9MSNfPTDTTZKla69qTbugHhWZnDg';
        const parkCode = 'glac';
        const container = document.getElementById('alert-container');

        async function fetchAlerts() {
            try {
                const response = await fetch(`https://developer.nps.gov/api/v1/alerts?parkCode=${parkCode}&api_key=${apiKey}`);
                const result = await response.json();

                // Clear the "Loading" text
                container.innerHTML = `<h2>Glacier National Park Status</h2>`;

                if (result.data.length === 0) {
                    container.innerHTML += '<p>No active alerts at this time.</p>';
                    return;
                }

                result.data.forEach(alert => {
                    // Create the HTML for each alert
                    const card = document.createElement('div');

                    // Add classes for styling (Danger, Caution, etc.)
                    const categoryClass = alert.category.toLowerCase().replace(/\s+/g, '-');
                    card.className = `alert-card ${categoryClass}`;

                    card.innerHTML = `
                        <span class="category-badge">${alert.category}</span>
                        <h2>${alert.title}</h2>
                        <p>${alert.description}</p>
                    `;
                    container.appendChild(card);
                });
            } catch (error) {
                container.innerHTML = `<p style="color:red;">Error loading alerts. Please try again later.</p>`;
                console.error(error);
            }
        }

        fetchAlerts();
</script>