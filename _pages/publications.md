---
layout: page
permalink: /publications/
title: Publications
description: Zhuozheng's works. For a full list of publications, <a href='https://scholar.google.com/citations?user=YS4hr1UAAAAJ&hl=us-EN'>Click here</a>!
years: [2023,2022,2021]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>