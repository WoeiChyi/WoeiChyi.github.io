---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div style="text-align: justify; text-justify: inter-word;">
  This is Woei-Chyi, and I am currently working as a Postdoctoral Researcher at Purdue University. I received my Ph.D. in Civil Engineering (under supervision of Prof. Hasanzadeh) and M.S. in Electrical and Computer Engineering at Purdue University. My research focuses on Human-Autonomy Teaming, Digital Twins, Data Science, Wearable Sensing, Human Factors, and AR/VR/XR/MR. I have been working on multiple interdisciplinary research projects funded by the National Science Foundation (NSF), U.S. Department of Transportation (USDOT), and Indiana Department of Transportation (INDOT) in collaboration with experts across domains. The findings have been translated into journal articles, conference proceedings, and technical reports.
</div>

<!-- Leaflet CSS + JS -->
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
  integrity="sha256-o88AwQnXNh2a1lGgU1rqkpo4wAlGpG8lqIehudM+5mY=" crossorigin="" />
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
  integrity="sha256-o9N1j9Azl7Z4Q3NH6tK04l4J98KjJyfGLv0hZNDbs14=" crossorigin=""></script>

<!-- Map container with full width -->
<div id="map" style="height: 500px; width: 100%; margin-top: 2em;"></div>

<script>
  // Initialize map
  var map = L.map('map').setView([20, 0], 2); // World view

  // Add OpenStreetMap tile layer
  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright" target="_blank">OpenStreetMap</a> contributors',
    maxZoom: 18
  }).addTo(map);

  // Add example markers
  L.marker([40.4237, -86.9212]).addTo(map).bindPopup('Purdue University');
  L.marker([37.7749, -122.4194]).addTo(map).bindPopup('San Francisco - Conference');

  // Fix for rendering issues in some templates
  setTimeout(function () {
    map.invalidateSize();
  }, 500);
</script>
