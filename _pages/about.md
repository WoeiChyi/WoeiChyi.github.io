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

<!-- Add Leaflet Map -->
<link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
<script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>

<div id="map" style="height: 500px; margin-top: 2em;"></div>

<script>
  var map = L.map('map').setView([20, 0], 2); // World view

  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '© OpenStreetMap contributors'
  }).addTo(map);

  // Example markers (customize with your places)
  L.marker([40.4237, -86.9212]).addTo(map).bindPopup('Purdue University');
  L.marker([37.7749, -122.4194]).addTo(map).bindPopup('San Francisco - Conference');
</script>
