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

<div style="margin-top: 2em;">
  <h2 style="margin-bottom: 0.5em;">Education</h2>
  <ul style="list-style: disc; padding-left: 1.5em; text-align: justify; text-justify: inter-word;">
    <li><strong>Ph.D. in Civil Engineering</strong>, Purdue University, USA (2021-2025)</li>
    <li><strong>M.S. in Electrical and Computer Engineering</strong>, Purdue University, USA (2024-2025)</li>
    <li><strong>Exchange in Civil and Environmental Engineering</strong>, TU Darmstadt, Germany (2019-2020)</li>
    <li><strong>M.S. in Civil Engineering</strong>, National Taiwan University, Taiwan (2017-2020)</li>
    <li><strong>B.S. in Civil Engineering</strong>, National Taiwan University, Taiwan (2013-2017)</li>
  </ul>
</div>

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<div id="map" style="height: 500px; width: 100%; margin-top: 2em;"></div>

<script>
  var map = L.map('map').setView([40.4237, 20], 2);

  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors',
    maxZoom: 18,
  }).addTo(map);

  L.marker([40.4237, -86.9212]).addTo(map).bindPopup('Purdue University');
  L.marker([25.0173, 121.5398]).addTo(map).bindPopup('National Taiwan University');
  L.marker([49.8719, 8.6512]).addTo(map).bindPopup('TU Darmstadt');

  setTimeout(function () {
    map.invalidateSize();
  }, 500);
</script>
