---
layout: page
title: Archaeology
permalink: /archaeology/
---
I hold a bachelor's degree in anthropology from the University of Michigan. While I was trained in four-field anthropology, my area of focus was in archaeology. 

## Field Work

- Maya Research Program, Blue Creek, Belize, 2012
- Khirbet Iskander Expedition, Madaba, Jordan, 2013
- Field School in Athabaskan Prehistory, Delta Junction, Alaska, 2016

## News Test

<div id="news-container">
    <p>Loading the latest stories...</p>
</div>

<script>
async function loadRecentNews() {
    try {
        // 1. Fetch the data from your JSON file
        const response = await fetch('news.json');
        const data = await response.json();

        // 2. Take only the first 5 items
        const recentStories = data.slice(0, 5);

        // 3. Find the container on your page
        const container = document.getElementById('news-container');

        // 4. Map through the data and create HTML
        container.innerHTML = recentStories.map(story => `
            <div class="news-item">
                <a href="${story.url}" target="_blank">${story.title}</a>
            </div>
        `).join('');

    } catch (error) {
        console.error('Error loading the news:', error);
    }
}

// Call the function when the page loads
loadRecentNews();
</script>