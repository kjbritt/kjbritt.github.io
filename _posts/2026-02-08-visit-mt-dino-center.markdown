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

You can visit the Montana Dinosaur Center this summer.


<div id="alert-container">
        <h1>Glacier National Park Status</h1>
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
                container.innerHTML = `<h1>Glacier National Park Status</h1>`;

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